---
title: S/MIME v programu Outlook v spletu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772314"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="5db50-102">Šifriranje e-poštnih sporočil v Outlooku</span><span class="sxs-lookup"><span data-stu-id="5db50-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="5db50-103">Šifriranje sporočil v storitvi Microsoft 365 je zgrajeno na Microsoft Azure Rights Management (Azure RMS), ki je del zaščite informacij Azure.</span><span class="sxs-lookup"><span data-stu-id="5db50-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="5db50-104">Če vaša naročnina vključuje upravljanje pravic v storitvi Azure ali Azure, **vam ni treba izvesti nobenih dejanj, s katerimi lahko ročno omogočite ali aktivirate** storitev za upravljanje pravic.</span><span class="sxs-lookup"><span data-stu-id="5db50-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="5db50-105">Na podlagi povratnih informacij strank vam ne bomo več omogočili pravil pretoka pošte Exchange za samodejno šifriranje odhodnih e-poštnih sporočil, ki vsebujejo določeno vrsto občutljivih informacij v najemniku.</span><span class="sxs-lookup"><span data-stu-id="5db50-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="5db50-106">Namesto tega zagotavljamo podrobna navodila o tem, kako lahko to naredite sami.</span><span class="sxs-lookup"><span data-stu-id="5db50-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="5db50-107">Če želite več podrobnosti o tem, kako ustvarite pravilo prenosa za šifriranje občutljivih informacij, si oglejte [Ta članek](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="5db50-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="5db50-108">Če uporabljate Outlook v spletu (prej **OWA**): pri sestavljanju e-poštnega sporočila preprosto kliknite **zaščiti** v programu owa.</span><span class="sxs-lookup"><span data-stu-id="5db50-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="5db50-109">S tem boste uporabili dovoljenje» ne Posreduj «.</span><span class="sxs-lookup"><span data-stu-id="5db50-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="5db50-110">Kliknite **Spremeni dovoljenje** in izberite **Šifriraj** , da le šifrirate sporočilo.</span><span class="sxs-lookup"><span data-stu-id="5db50-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="5db50-111">Če uporabljate **Outlook Client**: Če želite poslati šifrirano sporočilo iz Outlooka 2013 ali 2016 ali Outlook 2016 za Mac, izberite **možnosti**  >  **dovoljenja**, nato pa izberite možnost zaščite, ki jo potrebujete.</span><span class="sxs-lookup"><span data-stu-id="5db50-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="5db50-112">Če želite **samodejno šifrirati vso e-pošto** , poslano nekaterim prejemnikom ali zunanjim partnerjem, morate ustvariti pravilo prenosa pošte v skrbniškem središču za Exchange.</span><span class="sxs-lookup"><span data-stu-id="5db50-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="5db50-113">Podrobna navodila so na voljo v [tem članku podpore](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="5db50-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

