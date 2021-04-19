---
title: Ali so vaši uporabniki prejeli e-pošto z zlonamerno vsebino?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815262"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="e3dcb-102">Ali so vaši uporabniki prejeli e-pošto z zlonamerno vsebino?</span><span class="sxs-lookup"><span data-stu-id="e3dcb-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="e3dcb-103">E-pošto z zlonamerno vsebino lahko odslej prijavite Microsoftu s [skrbniškimi pošiljkami v središču za varnost in skladnost s predpisi](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="e3dcb-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="e3dcb-104">Sporočila, ki so poslana v [skrbniških pošiljkah](https://sip.protection.office.com/reportsubmission), so pregledane, v pojavnem oknu s **podrobnostmi** pa so prikazani ti rezultati:</span><span class="sxs-lookup"><span data-stu-id="e3dcb-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="e3dcb-105">Če je prišlo do napake v preverjanju pristnosti e-poštnega naslova pošiljatelja ob trenutku dostave.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="e3dcb-106">Informacije o morebitnih zadetkih pravilnika, ki bi lahko vplivale na odločitev o sporočilu ali pa bi jo preglasile.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="e3dcb-107">S trenutno detonacijo je prikazano, ali so bili URL-ji ali datoteke, ki so bile v sporočilu, zlonamerne ali ne.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="e3dcb-108">Povratne informacije ocenjevalcev</span><span class="sxs-lookup"><span data-stu-id="e3dcb-108">Feedback from graders</span></span>

<span data-ttu-id="e3dcb-109">Če je bila zaznana preglasitev, bi moral biti v nekaj minutah dokončan vnovični pregled.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="e3dcb-110">Če ni prišlo do težave pri preverjanju pristnosti ali če na dostavo ni vplivala preglasitev, bi lahko povratne informacije ocenjevalcev trajale do enega dne.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="e3dcb-111">Če se ne strinjate s končno oceno sporočila, URL-ja ali datoteke (blokirano ali neblokirano), po enem dnevu znova pošljite sporočilo za vnovični pregled.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="e3dcb-112">Obstaja velika verjetnost, da bo ocena sporočila po vnovični pošiljki drugačna.</span><span class="sxs-lookup"><span data-stu-id="e3dcb-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="e3dcb-113">Medtem lahko zlonamerno e-pošto odstranite iz uporabniških nabiralnikov tako, da upoštevate navodila v [tem članku](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="e3dcb-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="e3dcb-114">Stranke s platformo Microsoft Defender za Office 365 lahko izvajajo ta opravila:</span><span class="sxs-lookup"><span data-stu-id="e3dcb-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="e3dcb-115">uporabijo [Raziskovalca groženj za iskanje in brisanje sumljive e-pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered),</span><span class="sxs-lookup"><span data-stu-id="e3dcb-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="e3dcb-116">[uporabijo Varne povezave za blokiranje dostopa](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) do zlonamernega URL-ja,</span><span class="sxs-lookup"><span data-stu-id="e3dcb-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="e3dcb-117">sledijo uporabnikom, ki so kliknili zlonamerne URL-je in dostopali do njih: [ogled URL-jev lažnega predstavljanja in klik za oceno o podatkih](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace),</span><span class="sxs-lookup"><span data-stu-id="e3dcb-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="e3dcb-118">ročno [začnejo avtomatizirano preiskavo](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).</span><span class="sxs-lookup"><span data-stu-id="e3dcb-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="e3dcb-119">Lahko tudi uporabite zaščito pred zlonamernimi datotekami in URL-ji tako, da upoštevate navodila v razdelku [Zaščita pred zlonamernimi URL-ji in datotekami](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="e3dcb-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>