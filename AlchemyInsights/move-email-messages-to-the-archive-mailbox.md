---
title: E-poštnih sporočil premakniti arhivskega nabiralnika
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418341"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="16ba4-102">Premakniti email arhivskega nabiralnika</span><span class="sxs-lookup"><span data-stu-id="16ba4-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="16ba4-103">Potrditev, da je bila omogočena **Arhiv nabiralnik** .</span><span class="sxs-lookup"><span data-stu-id="16ba4-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="16ba4-104">V nasprotnem primeru, sledite korakom v [tem članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) za omogočanje arhivskega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="16ba4-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="16ba4-105">V arhiv sporočil samodejno arhivskega nabiralnika, oznako za hranjenje z dejanjem **Premakni v Arhiv** mora biti nastavljena na **samodejno dodati oznako celoten predal (privzeto)**.</span><span class="sxs-lookup"><span data-stu-id="16ba4-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="16ba4-106">Sledite korakom tukaj ustvariti oznako: [Arhiv privzeto oznako](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="16ba4-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="16ba4-107">Nato dodajte oznako **Arhiv** pravilnik o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="16ba4-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="16ba4-108">V skrbniškem središču za izmenjavo, izberite **Zadrževanja** > dodati, **premakniti za oznako Arhiv** politike >, **shranite**.</span><span class="sxs-lookup"><span data-stu-id="16ba4-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="16ba4-109">Zdaj [dodelite pravilnik o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) posebne uporabnikovega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="16ba4-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="16ba4-110">Istega pravilnika veljajo na **primarnega** in **arhivskega** nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="16ba4-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="16ba4-111">Je potrebno za vsiljevanje uspelo mapo pomočnika (MFA) teči ter uveljavil nove nastavitve uporabnikovega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="16ba4-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="16ba4-112">Zaženite ta ukaz, medtem ko [povezati EKSO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) začeti pomočnik za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="16ba4-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="16ba4-113">Če želite več informacij o nastavljanju pravilnik arhiviranja, glejte [Nastavitev Arhiv in izbris pravilnika za nabiralnike](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="16ba4-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

