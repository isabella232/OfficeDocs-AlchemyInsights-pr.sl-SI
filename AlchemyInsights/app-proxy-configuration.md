---
title: Konfiguracija proxyja aplikacije
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885528"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="299a4-102">Konfiguracija proxyja aplikacije</span><span class="sxs-lookup"><span data-stu-id="299a4-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="299a4-103">Če želite razumeti, kako konfigurirate program proxy programa v storitvi Azure AD, da razkrijete aplikacije na mestu uporabe v oblaku, glejte [Kako konfigurirate program proxy programa](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="299a4-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="299a4-104">Enotna prijava (SSO) uporabnikom omogoča dostop do aplikacije brez preverjanja pristnosti večkrat.</span><span class="sxs-lookup"><span data-stu-id="299a4-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="299a4-105">Omogoča enotno preverjanje pristnosti, ki se pojavi v oblaku, proti imeniku Azure Active Directory, in dovoljuje storitvi ali povezovalniku, da pozove uporabnika, da dokonča vse dodatne izzive preverjanja pristnosti iz aplikacije.</span><span class="sxs-lookup"><span data-stu-id="299a4-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="299a4-106">Če želite izvedeti več, si oglejte [kako konfigurirati enotno prijavo v program proxy programa](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="299a4-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="299a4-107">S [tem člankom](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) lahko odpravite težave s pogostimi težavami, ko ustvarjate nov program proxy strežnika.</span><span class="sxs-lookup"><span data-stu-id="299a4-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="299a4-108">Če imate težave z vzpostavljanjem preverjanja pristnosti, ki je na voljo v aplikaciji, boste morda morali [odpraviti omejitve dodeljevanja strežnikov Kerberos za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ali pa upoštevajte navodila za [konfiguracijo aplikacije s PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) , da odpravite težavo.</span><span class="sxs-lookup"><span data-stu-id="299a4-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
