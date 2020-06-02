---
title: Pravilniki o hranjenju v skrbniškem središču za Exchange ne delujejo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502623"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="abdc7-102">Pravilniki o hranjenju v skrbniškem središču Exchange</span><span class="sxs-lookup"><span data-stu-id="abdc7-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="abdc7-103">**Vprašanje:** Na novo ustvarjene ali posodobljene pravilnike o hranjenju v skrbniškem središču za Exchange se ne uporabljajo za nabiralnike ali artikle, ki niso premaknjeni v arhivski nabiralnik ali izbrisani.</span><span class="sxs-lookup"><span data-stu-id="abdc7-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="abdc7-104">**Temeljni vzroki:**</span><span class="sxs-lookup"><span data-stu-id="abdc7-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="abdc7-105">To je morda zato, ker **pomočnik za upravljane mape** ni obdelal uporabnikovega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="abdc7-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="abdc7-106">Pomočnik za upravljane mape poskuša obdelati vsak nabiralnik v organizaciji v oblaku vsakih sedem dni.</span><span class="sxs-lookup"><span data-stu-id="abdc7-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="abdc7-107">Če spremenite oznako za hranjenje ali v nabiralnik uporabite drug pravilnik o hranjenju, lahko počakate, da postopek pomoči za upravljano mapo obdela nabiralnik, lahko pa zaženete ukaz» cmdlet «Start-ManagedFolderAssistant, da zaženete pomočnika za upravljane mape, da obdela določen nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="abdc7-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="abdc7-108">Zagon tega ukaza» cmdlet «je uporaben za preskušanje ali odpravljanje težav z nastavitvami pravilnika o hranjenju ali oznake za hranjenje.</span><span class="sxs-lookup"><span data-stu-id="abdc7-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="abdc7-109">Če želite več informacij, preberite [zagon pomočnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="abdc7-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="abdc7-110">**Rešitev:** Zaženite ta ukaz, da zaženete pomočnika za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="abdc7-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="abdc7-111">To se lahko zgodi tudi, če je bil v nabiralniku **omogočen** **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="abdc7-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="abdc7-112">Če je bil nabiralnik postavljen na RetentionHold, pravilnik o hranjenju v nabiralniku v tem času ne bo obdelan.</span><span class="sxs-lookup"><span data-stu-id="abdc7-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="abdc7-113">Za več informacij o nastavitvi RetentionHold glejte: [zadržanje hranjenja nabiralnika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="abdc7-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="abdc7-114">**Rešitev:**</span><span class="sxs-lookup"><span data-stu-id="abdc7-114">**Solution:**</span></span>
    
  - <span data-ttu-id="abdc7-115">Preverite stanje nastavitve RetentionHold v določenem nabiralniku v [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="abdc7-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="abdc7-116">Zaženite ta ukaz, da **onemogočite** RetentionHold v določenem nabiralniku:</span><span class="sxs-lookup"><span data-stu-id="abdc7-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="abdc7-117">Zdaj znova zaženite pomočnika za upravljane mape:</span><span class="sxs-lookup"><span data-stu-id="abdc7-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="abdc7-118">**Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="abdc7-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="abdc7-119">Če želite več informacij o pravilnikih hranjenja v skrbniškem središču za Exchange, glejte:</span><span class="sxs-lookup"><span data-stu-id="abdc7-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="abdc7-120">Oznake za hranjenje in pravilniki o hranjenju</span><span class="sxs-lookup"><span data-stu-id="abdc7-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="abdc7-121">Uporaba pravilnika o hranjenju za nabiralnike</span><span class="sxs-lookup"><span data-stu-id="abdc7-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="abdc7-122">Dodajanje ali odstranjevanje oznak za hranjenje</span><span class="sxs-lookup"><span data-stu-id="abdc7-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="abdc7-123">Kako prepoznati vrsto zadržanja, danega v nabiralnik</span><span class="sxs-lookup"><span data-stu-id="abdc7-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
