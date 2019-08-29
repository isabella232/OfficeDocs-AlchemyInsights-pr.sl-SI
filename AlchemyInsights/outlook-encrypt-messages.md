---
title: S/MIME v Outlook v spletu
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666856"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="341b3-102">Šifriranje e-poštnih sporočil v Outlook</span><span class="sxs-lookup"><span data-stu-id="341b3-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="341b3-103">Šifriranje sporočil Office 365 temelji na Microsoft Azure Rights Management (Azure RMS), ki je del Azure varovanja informacij.</span><span class="sxs-lookup"><span data-stu-id="341b3-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="341b3-104">Če vaša naročnina vključuje Azure IRM ali Azure varovanja informacij, **vam ni treba sprejeti vse ukrepe za ročno omogočite ali aktivirati** storitev upravljanja pravic.</span><span class="sxs-lookup"><span data-stu-id="341b3-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="341b3-105">Glede na povratne informacije strank, smo bo ne usposobiti tok pravila izmenjave pošte samodejno šifrira namenjen ven email, ki vsebuje določene vrste občutljivih informacij v vašem najemnik privzeto.</span><span class="sxs-lookup"><span data-stu-id="341b3-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="341b3-106">Namesto tega, nudimo podrobna navodila o tem, kako lahko to storite sami.</span><span class="sxs-lookup"><span data-stu-id="341b3-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="341b3-107">Dodatne podrobnosti o tem, kako ustvarite pravila prenosa za šifriranje občutljivih podatkov, glejte [Ta članek](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="341b3-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="341b3-108">Če uporabljate Outlook v spletu (prej **OWA**): ko skladanjem email vest, preprosto kliknite **zaščiti** v OWA.</span><span class="sxs-lookup"><span data-stu-id="341b3-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="341b3-109">To bo veljalo "Do not forward" dovoljenje.</span><span class="sxs-lookup"><span data-stu-id="341b3-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="341b3-110">Kliknite **Spremeni dovoljenje** in izberete **Šifriraj** samo šifrirali sporočilo.</span><span class="sxs-lookup"><span data-stu-id="341b3-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="341b3-111">Če uporabljate **Outlookov odjemalec**: pošiljanje šifriranega sporočila iz Outlooka, 2013 ali 2016, ali Outlook 2016 za Mac, da izberete **možnosti** > **dovoljenja**, nato pa izberite želeno možnost zaščite.</span><span class="sxs-lookup"><span data-stu-id="341b3-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="341b3-112">**Samodejno šifrirajo vsi email** pošlje nekaterih prejemnikov ali zunanje partnerske organizacije, morate ustvariti praviloma pošta pretok prometa v skrbniškem središču za izmenjavo.</span><span class="sxs-lookup"><span data-stu-id="341b3-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="341b3-113">Podrobna navodila v [članku s pomočjo](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="341b3-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

