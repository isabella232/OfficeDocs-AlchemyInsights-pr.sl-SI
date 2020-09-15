---
title: Prepoznavanje zunanjega posredovanja e-pošte v nabiralnikih v dnevnikih nadzora
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696313"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="d0e20-102">Prepoznavanje, ko je zunanja e-poštna preusmeritev konfigurirana v nabiralnikih</span><span class="sxs-lookup"><span data-stu-id="d0e20-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="d0e20-103">Ko uporabnik programa Microsoft 365 konfigurira zunanjo posredovanje e-pošte v nabiralniku, je dejavnost revidirana kot del ukaza» cmdlet « **set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="d0e20-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="d0e20-104">V središču za skladnost varnosti & lahko vidite dejavnost z iskanjem dnevnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="d0e20-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="d0e20-105">Prijavite se v središče za preverjanje [varnosti & za skladnost s predpisi Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="d0e20-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="d0e20-106">Pojdite na stran **Search**  >  **iskanje dnevnika nadzora** iskanja.</span><span class="sxs-lookup"><span data-stu-id="d0e20-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="d0e20-107">Izberite datumski obseg v poljih **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="d0e20-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d0e20-108">Ni vam treba določiti uporabniškega imena.</span><span class="sxs-lookup"><span data-stu-id="d0e20-108">You don't need to specify a username.</span></span> <span data-ttu-id="d0e20-109">Preverite, ali je polje **dejavnosti** nastavljeno tako, da **prikazuje rezultate za vse dejavnosti**.</span><span class="sxs-lookup"><span data-stu-id="d0e20-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="d0e20-110">Kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="d0e20-110">Click **Search**.</span></span>

<span data-ttu-id="d0e20-111">V rezultatih kliknite **Filtriraj rezultate** in vnesite **nabiralnik** v polje Filter dejavnosti.</span><span class="sxs-lookup"><span data-stu-id="d0e20-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="d0e20-112">V rezultatih Izberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="d0e20-112">Select an audit record in the results.</span></span> <span data-ttu-id="d0e20-113">V razdelku **podrobnosti** flyout kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="d0e20-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="d0e20-114">Če želite ugotoviti, ali je dejavnost povezana z odpošiljanjem e-pošte, si morate ogledati podrobnosti posameznega revizijskega zapisa.</span><span class="sxs-lookup"><span data-stu-id="d0e20-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="d0e20-115">**Objectid**: vrednost vzdevka nabiralnika, ki je bil spremenjen.</span><span class="sxs-lookup"><span data-stu-id="d0e20-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="d0e20-116">**Parametri**: _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.</span><span class="sxs-lookup"><span data-stu-id="d0e20-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="d0e20-117">**ID**uporabnika: uporabnik, ki je konfiguriral posredovanje e-pošte v nabiralniku v polju» **objectid** «.</span><span class="sxs-lookup"><span data-stu-id="d0e20-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="d0e20-118">Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d0e20-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
