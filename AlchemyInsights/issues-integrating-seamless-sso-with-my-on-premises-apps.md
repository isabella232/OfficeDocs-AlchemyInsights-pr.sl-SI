---
title: Težave z integracijo brezšivne SSO s programi na mestu uporabe
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868724"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="f1b39-102">Težave z integracijo brezšivne SSO s programi na mestu uporabe</span><span class="sxs-lookup"><span data-stu-id="f1b39-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="f1b39-103">Če želite odpraviti težave z integracijo brezšivne SSO s programi na mestu uporabe, naredite to:</span><span class="sxs-lookup"><span data-stu-id="f1b39-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="f1b39-104">**Priporočeni koraki**</span><span class="sxs-lookup"><span data-stu-id="f1b39-104">**Recommended steps**</span></span>

1. <span data-ttu-id="f1b39-105">Če želite konfigurirati **program na** mestu uporabe za **enotno prijavo prek proxya programa**, si oglejte [Iskanje gesla za enotno prijavo s proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="f1b39-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="f1b39-106">**Odpravljanje težav s proxyjem aplikacije**: priporočamo, da začnete s pregledovanjem toka odpravljanja težav, [težav s povezovalnikom strežnika debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), če želite ugotoviti, ali so povezovalniki proxy programov pravilno konfigurirani.</span><span class="sxs-lookup"><span data-stu-id="f1b39-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="f1b39-107">Če imate še vedno težave z vzpostavljanjem povezave z aplikacijo, upoštevajte navodila za odpravljanje težav v aplikaciji [aplikacije proxy programa debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="f1b39-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="f1b39-108">Težave z [CORS lahko prepoznate](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) tako, da uporabite ta orodja za iskanje napak brskalnika:</span><span class="sxs-lookup"><span data-stu-id="f1b39-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="f1b39-109">Zaženite brskalnik in prebrskajte do spletnega programa.</span><span class="sxs-lookup"><span data-stu-id="f1b39-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="f1b39-110">Pritisnite **F12** , da prikažete konzolo Debug.</span><span class="sxs-lookup"><span data-stu-id="f1b39-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="f1b39-111">Poskusite znova ustvariti transakcijo in preglejte konzolno sporočilo.</span><span class="sxs-lookup"><span data-stu-id="f1b39-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="f1b39-112">Zaradi kršitve CORS se prikaže konzolna napaka o poreklu.</span><span class="sxs-lookup"><span data-stu-id="f1b39-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="f1b39-113">Nekaterih težav z CORS ni mogoče razrešiti, na primer, ko se aplikacija preusmeri v login.microsoftonline.com za preverjanje pristnosti, in je žeton za dostop potekel.</span><span class="sxs-lookup"><span data-stu-id="f1b39-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="f1b39-114">Klic CORS nato spodleti.</span><span class="sxs-lookup"><span data-stu-id="f1b39-114">The CORS call then fails.</span></span> <span data-ttu-id="f1b39-115">Rešitev tega scenarija je, da podaljšate življenjsko dobo Accessovega žetona, da preprečite, da bi poteklo med sejo uporabnika.</span><span class="sxs-lookup"><span data-stu-id="f1b39-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="f1b39-116">Če želite več informacij o tem, kako to naredite, glejte [Doživljenjska doba žetonov v Microsoftovi platformi za identiteto](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="f1b39-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="f1b39-117">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="f1b39-117">**Recommended documents**</span></span>

- [<span data-ttu-id="f1b39-118">Kako konfigurirati enotno prijavo v aplikacijo proxy programa</span><span class="sxs-lookup"><span data-stu-id="f1b39-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="f1b39-119">SAML enotne prijave za aplikacije na mestu uporabe z proxyjem programa</span><span class="sxs-lookup"><span data-stu-id="f1b39-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="f1b39-120">Razumevanje in reševanje težav z proxyjem storitve Azure Active Directory CORS</span><span class="sxs-lookup"><span data-stu-id="f1b39-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="f1b39-121">Odpravljanje težav s omejena konfiguracija dodeljevanja Kerberos za proxy programa</span><span class="sxs-lookup"><span data-stu-id="f1b39-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)