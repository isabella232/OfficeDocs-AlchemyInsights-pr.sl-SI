---
title: Prepoznavanje zunanjega posredovanja e-pošte v nabiralnikih v dnevnikih revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508968"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="d9079-102">Ugotovite, kdaj je zunanje posredovanje e-pošte konfigurirano v nabiralnikih</span><span class="sxs-lookup"><span data-stu-id="d9079-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="d9079-103">Ko uporabnik Microsoft 365 konfigurira zunanje posredovanje e-pošte v nabiralniku, se dejavnost revidira kot del ukaza» cmdlet « **set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="d9079-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="d9079-104">Dejavnost lahko vidite s pomočjo iskanja dnevnika revizij v središču za skladnost varnostnega &.</span><span class="sxs-lookup"><span data-stu-id="d9079-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="d9079-105">Prijavite se v [Microsoft 365 Security & center za skladnost](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="d9079-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="d9079-106">Pojdite na stran **Search**za  >  **iskanje dnevnika revizij** iskanja.</span><span class="sxs-lookup"><span data-stu-id="d9079-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="d9079-107">Izberite časovno območje v polji **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="d9079-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d9079-108">Uporabniškega imena ni treba določiti.</span><span class="sxs-lookup"><span data-stu-id="d9079-108">You don't need to specify a username.</span></span> <span data-ttu-id="d9079-109">Preverite, ali je polje **dejavnosti** nastavljeno tako, da **prikazuje rezultate za vse dejavnosti**.</span><span class="sxs-lookup"><span data-stu-id="d9079-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="d9079-110">Kliknite **Iskanje**.</span><span class="sxs-lookup"><span data-stu-id="d9079-110">Click **Search**.</span></span>

<span data-ttu-id="d9079-111">V rezultatih kliknite **filter rezultati** in vrsta **set-poštni nabiralnik** v filter dejavnosti škatla.</span><span class="sxs-lookup"><span data-stu-id="d9079-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="d9079-112">V rezultatih Izberite zapis o reviziji.</span><span class="sxs-lookup"><span data-stu-id="d9079-112">Select an audit record in the results.</span></span> <span data-ttu-id="d9079-113">V pojavnem meniju **podrobnosti** kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="d9079-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="d9079-114">Če želite ugotoviti, ali je dejavnost povezana s posredovanjem e-pošte, morate pogledati podrobnosti vsakega revizijskega zapisa.</span><span class="sxs-lookup"><span data-stu-id="d9079-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="d9079-115">**Objectid**: vrednost vzdevka nabiralnika, ki je bil spremenjen.</span><span class="sxs-lookup"><span data-stu-id="d9079-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="d9079-116">**Parametri**: _forwardingsmtpaddress_ označuje ciljni e-poštni naslov.</span><span class="sxs-lookup"><span data-stu-id="d9079-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="d9079-117">**Userid**: uporabnik, ki je konfiguriral posredovanje e-pošte v nabiralniku v polju **objectid** .</span><span class="sxs-lookup"><span data-stu-id="d9079-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="d9079-118">Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d9079-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
