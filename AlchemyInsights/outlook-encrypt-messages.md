---
title: S/MIME v programu Outlook na spletu
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752876"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="25ce0-102">Šifriranje e-poštnih sporočil v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="25ce0-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="25ce0-103">Šifriranje sporočil sistema Office 365 je zgrajeno v programu Microsoft Azure Rights Management (Azure RMS), ki je del programa Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="25ce0-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="25ce0-104">Če vaša naročnina vključuje upravljanje pravic Azure ali varstvo podatkov Azure, **vam ni treba sprejeti nobenih dejanj za ročno Omogočanje ali aktiviranje** storitve za upravljanje pravic.</span><span class="sxs-lookup"><span data-stu-id="25ce0-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="25ce0-105">Na podlagi povratnih informacij strank ne bomo več omogočali pravil o pretoku pošte Exchange za samodejno šifriranje odhodne e-pošte, ki vsebuje določene vrste občutljivih podatkov v vašem najemniku privzeto.</span><span class="sxs-lookup"><span data-stu-id="25ce0-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="25ce0-106">Namesto tega ponujamo podrobna navodila o tem, kako lahko to storite sami.</span><span class="sxs-lookup"><span data-stu-id="25ce0-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="25ce0-107">Če želite več podrobnosti o ustvarjanju pravila transporta za šifriranje občutljivih informacij, si oglejte [Ta članek](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="25ce0-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="25ce0-108">Če uporabljate Outlook v spletu (prej **OWA**): ko sestavljate e-poštno sporočilo, preprosto kliknite **zaščitite** v owa.</span><span class="sxs-lookup"><span data-stu-id="25ce0-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="25ce0-109">To bo veljalo za dovoljenje» ne Posreduj «.</span><span class="sxs-lookup"><span data-stu-id="25ce0-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="25ce0-110">Kliknite **Spremeni dovoljenje** in izberite **šifriranje** , da šifrirate samo sporočilo.</span><span class="sxs-lookup"><span data-stu-id="25ce0-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="25ce0-111">Če uporabljate **Outlook Client**: Če želite poslati šifrirano sporočilo iz Outlooka 2013 ali 2016 ali Outlook 2016 za Mac, izberite **možnosti** > **dovoljenja**, nato pa izberite možnost zaščite, ki jo potrebujete.</span><span class="sxs-lookup"><span data-stu-id="25ce0-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="25ce0-112">Če želite **samodejno šifrirati vso e-poštno sporočilo** , poslano nekaterim prejemnikom ali zunanjim partnerskim organizacijam, morate v skrbniškem središču za Exchange ustvariti pravilo za prenos pošte.</span><span class="sxs-lookup"><span data-stu-id="25ce0-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="25ce0-113">Podrobna navodila so na voljo v [tem članku za podporo](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="25ce0-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

