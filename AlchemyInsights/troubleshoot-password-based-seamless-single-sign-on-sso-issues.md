---
title: Odpravljanje težav z nemoteno enotno prijavo (SSO), ki temelji na geslih
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714887"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="3e92d-102">Odpravljanje težav z nemoteno enotno prijavo (SSO), ki temelji na geslih</span><span class="sxs-lookup"><span data-stu-id="3e92d-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="3e92d-103">Če želite izvedeti osnove funkcije SSO, ki temelji na geslih, glejte [preverjanje pristnosti, ki temelji na geslih, z imenikom Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="3e92d-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="3e92d-104">**Konfiguracija SSO, ki temelji na geslih**</span><span class="sxs-lookup"><span data-stu-id="3e92d-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="3e92d-105">[Konfiguracija enotne prijave na osnovi gesla](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – v tem članku je več podrobnosti o možnosti SSO, ki temelji na geslu.</span><span class="sxs-lookup"><span data-stu-id="3e92d-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="3e92d-106">Če program, ki ga želite dodati, zahteva konfiguracijo po meri in morate uporabiti SSO, ki temelji na geslih, je ta članek za vas.</span><span class="sxs-lookup"><span data-stu-id="3e92d-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="3e92d-107">[Konfiguracija enotne prijave na osnovi gesla za aplikacije on-Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – aplikacija proxy podpira več načinov enotne prijave.</span><span class="sxs-lookup"><span data-stu-id="3e92d-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="3e92d-108">Prijava na osnovi gesla je namenjena aplikacijam, ki uporabljajo kombinacijo uporabniškega imena in gesla za preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="3e92d-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="3e92d-109">Ko konfigurirate prijavo na osnovi gesla za vašo aplikacijo, se morajo uporabniki enkrat vpisati v program na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="3e92d-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="3e92d-110">V tem članku Azure Active Directory shranjuje informacije o vpisu in jih samodejno ponudi aplikaciji, ko vaši uporabniki dostopajo do njega na daljavo.</span><span class="sxs-lookup"><span data-stu-id="3e92d-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="3e92d-111">Aplikacijo morate že objaviti in preskusiti s proxyjem aplikacije.</span><span class="sxs-lookup"><span data-stu-id="3e92d-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="3e92d-112">V nasprotnem primeru upoštevajte navodila v razdelku [objavljanje programov s proxyjem storitve AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , nato pa nadaljujte s KONFIGURACIJO sistema SSO, ki temelji na geslu za aplikacije on-Prem.</span><span class="sxs-lookup"><span data-stu-id="3e92d-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="3e92d-113">Če želite odpraviti težave z geslom, ki temeljijo na geslu, glejte [Odpravljanje težav z enotno prijavo v storitvi AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="3e92d-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
