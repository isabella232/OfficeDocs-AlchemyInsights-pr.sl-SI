---
title: Omogočanje preverjanja pristnosti in odpravljanja težav SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077667"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="96a0a-102">Omogočanje preverjanja pristnosti in odpravljanja težav SMTP</span><span class="sxs-lookup"><span data-stu-id="96a0a-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="96a0a-103">Če želite omogočiti preverjanje pristnosti SMTP za nabiralnik ali pa se prikaže sporočilo o napaki »Odjemalska pristnost ni preverjena«, »Preverjanje pristnosti neuspešno« ali »SmtpClientAuthentication« s kodo 5.7.57 ali 5.7.3 ali 5.7.139, ko poskušate posredovati e-pošto s preverjanjem pristnosti naprave ali aplikacije s protokolom Microsoft 365, izvedite ta tri dejanja, da odpravite težavo:</span><span class="sxs-lookup"><span data-stu-id="96a0a-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="96a0a-104">Privzete nastavitve [varnosti Azure onemogočite tako,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) da možnost Omogoči **privzete nastavitve nastavite** na **Ne.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="96a0a-105">a.</span><span class="sxs-lookup"><span data-stu-id="96a0a-105">a.</span></span> <span data-ttu-id="96a0a-106">V portal Azure se vpišite kot skrbnik za varnost, skrbnik pogojnega dostopa ali globalni skrbnik.</span><span class="sxs-lookup"><span data-stu-id="96a0a-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="96a0a-107">b.</span><span class="sxs-lookup"><span data-stu-id="96a0a-107">b.</span></span> <span data-ttu-id="96a0a-108">Poiščite Azure Active Directory > **lastnosti.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="96a0a-109">c.</span><span class="sxs-lookup"><span data-stu-id="96a0a-109">c.</span></span> <span data-ttu-id="96a0a-110">Izberite **Upravljanje privzetih varnostnih nastavitev.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="96a0a-111">d.</span><span class="sxs-lookup"><span data-stu-id="96a0a-111">d.</span></span> <span data-ttu-id="96a0a-112">Nastavite **Omogoči privzete varnostne nastavitve** na **Ne.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="96a0a-113">e.</span><span class="sxs-lookup"><span data-stu-id="96a0a-113">e.</span></span> <span data-ttu-id="96a0a-114">Izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="96a0a-114">Select **Save**.</span></span>

2. <span data-ttu-id="96a0a-115">[Omogočanje pošiljanja SMTP odjemalca](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) v licenciranem nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="96a0a-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="96a0a-116">a.</span><span class="sxs-lookup"><span data-stu-id="96a0a-116">a.</span></span> <span data-ttu-id="96a0a-117">V Skrbniško središče za Microsoft 365 izberite **aktivni uporabniki** in izberite uporabnika.</span><span class="sxs-lookup"><span data-stu-id="96a0a-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="96a0a-118">b.</span><span class="sxs-lookup"><span data-stu-id="96a0a-118">b.</span></span> <span data-ttu-id="96a0a-119">Pojdite na zavihek Pošta in v razdelku **E-poštne aplikacije** izberite Upravljanje **e-poštnih aplikacij**.</span><span class="sxs-lookup"><span data-stu-id="96a0a-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="96a0a-120">d.</span><span class="sxs-lookup"><span data-stu-id="96a0a-120">d.</span></span> <span data-ttu-id="96a0a-121">Preverite, **ali je potrjeno polje SMTP s** preverjeno pristnostjo (omogočeno).</span><span class="sxs-lookup"><span data-stu-id="96a0a-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="96a0a-122">e.</span><span class="sxs-lookup"><span data-stu-id="96a0a-122">e.</span></span> <span data-ttu-id="96a0a-123">Izberite **Shrani spremembe.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="96a0a-124">[Onemogočite storitev Multi-Factor Authentication (MFA) v](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licenciranem nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="96a0a-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="96a0a-125">a.</span><span class="sxs-lookup"><span data-stu-id="96a0a-125">a.</span></span> <span data-ttu-id="96a0a-126">Pojdite na Skrbniško središče za Microsoft 365 in v levem meniju za krmarjenje izberite **Uporabniki**  >  **aktivni uporabniki.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="96a0a-127">b.</span><span class="sxs-lookup"><span data-stu-id="96a0a-127">b.</span></span> <span data-ttu-id="96a0a-128">Izberite **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="96a0a-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="96a0a-129">c.</span><span class="sxs-lookup"><span data-stu-id="96a0a-129">c.</span></span> <span data-ttu-id="96a0a-130">Izberite uporabnika in onemogočite **Multi-Factor auth.**</span><span class="sxs-lookup"><span data-stu-id="96a0a-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
