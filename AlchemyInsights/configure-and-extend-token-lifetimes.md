---
title: Konfiguracija in podaljšanje življenjske dobe žetona
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917012"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="ece49-102">Konfiguracija in podaljšanje življenjske dobe žetona</span><span class="sxs-lookup"><span data-stu-id="ece49-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="ece49-103">Določite lahko življenjsko dobo žetona Accessa, SAML ali ID-ja, ki ga je izdajala Microsoftova platforma za identiteto.</span><span class="sxs-lookup"><span data-stu-id="ece49-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="ece49-104">Življenjske dobe žetonov lahko nastavite za vse programe v organizaciji, za program multi-najemnika (multi-Organization) ali za določenega glavnega ponudnika v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="ece49-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="ece49-105">Če želite več informacij, preberite [trajanje veljavnosti žetonov](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes), ki jih je mogoče konfigurirati.</span><span class="sxs-lookup"><span data-stu-id="ece49-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="ece49-106">Za primere preberite [primere, kako konfigurirate življenjske dobe žetona](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="ece49-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="ece49-107">Če želite izvedeti, kako konfigurirate življenjsko dobo in združljivost žetona v storitvi Azure Active Directory B2C (Azure AD B2C), glejte [Konfiguracija žetonov v storitvi Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="ece49-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="ece49-108">V članku [konfigurirajte delovanje sej v storitvi Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) , v katerem so opisani načini enotne prijave (SSO), ki se uporabljajo v storitvi AZURE ad B2C in vam pomaga pri konfiguraciji pravilnika izbrati najprimernejšo metodo SSO.</span><span class="sxs-lookup"><span data-stu-id="ece49-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="ece49-109">**Kako dolgo trajajo žetoni? Kako dolgo veljajo?**</span><span class="sxs-lookup"><span data-stu-id="ece49-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="ece49-110">Življenjska doba žetonov je 1 ura in življenjska doba seje je 24 ur.</span><span class="sxs-lookup"><span data-stu-id="ece49-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="ece49-111">To pomeni, da se boste morali znova prijaviti, preden zaprosite za nov žeton, če v 24 urah ni bilo nobenih zahtev.</span><span class="sxs-lookup"><span data-stu-id="ece49-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="ece49-112">Po maju 30, 2020, noben novi najemnik ne bo mogel uporabiti pravilnika o življenjskem simbolu, ki ga je mogoče konfigurirati za konfiguracijo zasedanja in osveževanja žetonov.</span><span class="sxs-lookup"><span data-stu-id="ece49-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="ece49-113">Zastaranje se bo zgodilo v nekaj mesecih po tem, kar pomeni, da bomo ustavili čast obstoječega zasedanja in osvežili žetone policije.</span><span class="sxs-lookup"><span data-stu-id="ece49-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="ece49-114">Po zastaranju lahko še vedno konfigurirate življenjske dobe žetona za dostop.</span><span class="sxs-lookup"><span data-stu-id="ece49-114">You can still configure access token lifetimes after the deprecation.</span></span>






