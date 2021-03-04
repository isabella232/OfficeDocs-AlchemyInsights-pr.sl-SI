---
title: Odpravljanje težav z SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430214"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="88ca5-102">Odpravljanje težav z SSPR</span><span class="sxs-lookup"><span data-stu-id="88ca5-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="88ca5-103">**Imam težave pri konfiguraciji ponastavitev gesla**</span><span class="sxs-lookup"><span data-stu-id="88ca5-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="88ca5-104">Če ste skrbnik in si želite ogledati, kako omogočite samopostrežno ponastavitev gesla, glejte [Vadnica omogoči SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), da konfigurirate ponastavitev gesla za vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="88ca5-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="88ca5-105">Morda boste želeli pregledati tudi zahteve za [licenciranje](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="88ca5-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="88ca5-106">V vaši organizaciji morate dodeliti vsaj eno licenco.</span><span class="sxs-lookup"><span data-stu-id="88ca5-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="88ca5-107">**Samo uporabniki v oblaku** – vsak Office 365 (O365) plačan sku ali Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="88ca5-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="88ca5-108">**Uporabniki v oblaku in/ali na mestu uporabe** – Azure ad Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)</span><span class="sxs-lookup"><span data-stu-id="88ca5-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="88ca5-109">Če želite dodatna vprašanja o samopostrežnem ponastavitvi z geslom, si oglejte [naša vprašanja](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="88ca5-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="88ca5-110">**Dobivam sporočilo o napaki**</span><span class="sxs-lookup"><span data-stu-id="88ca5-110">**I'm getting an error message**</span></span>

<span data-ttu-id="88ca5-111">Oglejte si ta članek, če želite poiskati pogoste napake in njihove rešitve: [Odpravljanje težav z ponastavitvijo samopostrežnega gesla](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="88ca5-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="88ca5-112">**Imam težave s pravilnikom za ponastavitev gesla**</span><span class="sxs-lookup"><span data-stu-id="88ca5-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="88ca5-113">Če pravilnik za ponastavitev gesla ni v skladu s pričakovanji, ali če imate vprašanja o pravilnikih za ponastavitev gesla, si oglejte ta članek: [Pravilniki o geslih in omejitve v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="88ca5-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="88ca5-114">Pravilniki za ponastavitev gesla se ne nanašajo na skrbnike.</span><span class="sxs-lookup"><span data-stu-id="88ca5-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="88ca5-115">Microsoft uveljavi močne privzete pravilnike za ponastavitev gesla za vsako vlogo v storitvi Azure skrbnika.</span><span class="sxs-lookup"><span data-stu-id="88ca5-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="88ca5-116">Prepričajte se, da preizkušate uporabnika, ki ni skrbnik.</span><span class="sxs-lookup"><span data-stu-id="88ca5-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="88ca5-117">Če želite več informacij o pravilniku za ponastavitev skrbnika, si oglejte ta članek: [Ponastavi razlike pravilnika za skrbnike](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="88ca5-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="88ca5-118">**Ne želim, da moji uporabniki registrirajo dodatne varnostne informacije za ponastavitev gesla**</span><span class="sxs-lookup"><span data-stu-id="88ca5-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="88ca5-119">Za uporabnike lahko vnaprej zapolnite podatke (e-poštne in telefonske atribute), ki uporabljajo API, PowerShell ali Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="88ca5-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="88ca5-120">Če želite izvedeti, kako brati:</span><span class="sxs-lookup"><span data-stu-id="88ca5-120">To learn how read:</span></span>

- [<span data-ttu-id="88ca5-121">Uvajanje ponastavitev gesla brez zahteve za registracijo uporabnikov</span><span class="sxs-lookup"><span data-stu-id="88ca5-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="88ca5-122">Katere podatke uporablja ponastavitev gesla</span><span class="sxs-lookup"><span data-stu-id="88ca5-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="88ca5-123">**Želim, da moji uporabniki registrirajo svoje dodatne varnostne informacije za ponastavitev gesla**</span><span class="sxs-lookup"><span data-stu-id="88ca5-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="88ca5-124">Naj vaši uporabniki registrirajo svoje varnostne informacije za samoponastavitev gesla, tako da jih usmerjajo v [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="88ca5-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="88ca5-125">Ko so podatki poseljeni za uporabnika (uporabnik ali skrbnik), usmerite uporabnika v [aka.MS/sspr](https://passwordreset.microsoftonline.com/) , da bodo uporabniki lahko ponastavili svoja gesla.</span><span class="sxs-lookup"><span data-stu-id="88ca5-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="88ca5-126">Če uporabniki še vedno doživljajo težave, so uporabniki, ki so najverjetneje **združevali** ali **razpršili geslo, sinhronizirani** .</span><span class="sxs-lookup"><span data-stu-id="88ca5-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="88ca5-127">To pomeni, da je prišlo do težave z geslom storitve Nepotrjenim.</span><span class="sxs-lookup"><span data-stu-id="88ca5-127">This means there is likely a problem with the Password Writeback service.</span></span>