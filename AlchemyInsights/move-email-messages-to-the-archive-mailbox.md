---
title: E-poštnih sporočil premakniti arhivskega nabiralnika
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489987"
---
<span data-ttu-id="4d8da-p101">Težave, arhiviranje elementov v arhivski nabiralnik. Poskrbite, da boste izvedli naslednje korake:</span><span class="sxs-lookup"><span data-stu-id="4d8da-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="4d8da-p102">Potrditev, da je bila omogočena **Arhiv nabiralnik** . V nasprotnem primeru, sledite korakom v [tem članku](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) za omogočanje arhivskega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="4d8da-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="4d8da-106">V središču Admin Exchange izberite **Oznake za hranjenje** pod **Vodstvom, skladnost**, ustvariti **oznako za hranjenje** z dejanjem **premaknete Arhiv** , ki vsebuje želeno **Hranjenja**.</span><span class="sxs-lookup"><span data-stu-id="4d8da-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="4d8da-107">V skrbniškem središču Exchange, izberite **Pravilniki o hranjenju**, ustvarite **Pravilnik o hranjenju** in dodajte vaše **preseliti Arhiv** oznako za hranjenje politike.</span><span class="sxs-lookup"><span data-stu-id="4d8da-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="4d8da-p103">Za posebne uporabnikovega nabiralnika [dodelite pravilnik o hranjenju](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) . Istega pravilnika veljajo na **primarnega** in **arhivskega** nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="4d8da-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="4d8da-p104">Uporabnikovega nabiralnika se pravilnik arhiviranja, ki ga želite premikati elemente v arhivski nabiralnik. Je potrebno za vsiljevanje uspelo mapo pomočnika (MFA) teči ter uveljavil nove nastavitve uporabnikovega nabiralnika. Zaženite ta ukaz, medtem ko [povezati EKSO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) začeti pomočnik za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="4d8da-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="4d8da-113">Želite več informacij o vzpostavitvi pravilnik arhiviranja, glejte [Nastavitev Arhiv in izbris pravilnika za nabiralnike](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="4d8da-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

