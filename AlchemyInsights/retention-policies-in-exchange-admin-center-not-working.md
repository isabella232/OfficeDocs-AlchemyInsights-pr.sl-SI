---
title: Pravilniki o hranjenju v skrbniškem središču za Exchange ne delujejo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740526"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="2ff4d-102">Pravilniki o hranjenju v skrbniškem središču za Exchange</span><span class="sxs-lookup"><span data-stu-id="2ff4d-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="2ff4d-103">Če želite, da zaženemo avtomatizirane kontrole za spodaj navedene nastavitve, izberite gumb» Vrni «< na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s pravilniki o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="2ff4d-104">**Težava:** Novo ustvarjene ali posodobljene pravilnike o hranjenju v skrbniškem središču za Exchange se ne uporabljajo za nabiralnike ali elemente, ki niso premaknjeni v arhivski nabiralnik ali izbrisani.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="2ff4d-105">**Vzroki vzrokov:**</span><span class="sxs-lookup"><span data-stu-id="2ff4d-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="2ff4d-106">To je morda zato, ker **pomočnik za upravljane mape** ni obdelal nabiralnika uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="2ff4d-107">Pomočnik za upravljane mape poskuša obdelati vse nabiralnike v organizaciji v oblaku vsakih sedem dni.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="2ff4d-108">Če spremenite oznako za hranjenje ali v nabiralnik uporabite drug pravilnik o hranjenju, lahko počakate, da upravljana mapa pomaga pri obdelavi nabiralnika, lahko pa zaženete ukaz» cmdlet «Start-ManagedFolderAssistant, da zaženete pomočnika za upravljane mape za obdelavo določenega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="2ff4d-109">Zagon tega ukaza» cmdlet «je uporaben za preskušanje ali odpravljanje težav s pravilnikom o hranjenju ali postavljanjem oznak za hranjenje.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="2ff4d-110">Če želite več informacij, obiščite spletno mesto [Zaženi pomočnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="2ff4d-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="2ff4d-111">**Rešitev:** Zaženite ta ukaz, da zaženete pomočnika za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="2ff4d-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="2ff4d-112">Do tega lahko pride tudi, če je v nabiralniku **omogočeno** **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="2ff4d-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="2ff4d-113">Če je bil nabiralnik nameščen v RetentionHold, se pravilnik o hranjenju v nabiralniku v tem času ne bo obdelal.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="2ff4d-114">Če želite več namestitvi v nastavitvi RetentionHold, glejte: zadržanje [nabiralnika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="2ff4d-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="2ff4d-115">**Rešitev**</span><span class="sxs-lookup"><span data-stu-id="2ff4d-115">**Solution:**</span></span>
    
  - <span data-ttu-id="2ff4d-116">Preverite stanje nastavitve RetentionHold za določen nabiralnik v storitvi [ekso PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="2ff4d-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="2ff4d-117">Zaženite ta ukaz, če želite **onemogočiti** RetentionHold v določenem nabiralniku:</span><span class="sxs-lookup"><span data-stu-id="2ff4d-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="2ff4d-118">Zdaj znova zaženite pomočnika za upravljane mape:</span><span class="sxs-lookup"><span data-stu-id="2ff4d-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="2ff4d-119">**Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="2ff4d-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="2ff4d-120">Če želite več informacij o pravilnikih o hranjenju v skrbniškem središču za Exchange, glejte:</span><span class="sxs-lookup"><span data-stu-id="2ff4d-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="2ff4d-121">Oznake hranjenja in pravilniki o hranjenju</span><span class="sxs-lookup"><span data-stu-id="2ff4d-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="2ff4d-122">Uporaba pravilnika o hranjenju za nabiralnike</span><span class="sxs-lookup"><span data-stu-id="2ff4d-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="2ff4d-123">Dodajanje ali odstranjevanje oznak za hranjenje</span><span class="sxs-lookup"><span data-stu-id="2ff4d-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="2ff4d-124">Kako prepoznati vrsto zadržanja, ki je nameščena v nabiralniku</span><span class="sxs-lookup"><span data-stu-id="2ff4d-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
