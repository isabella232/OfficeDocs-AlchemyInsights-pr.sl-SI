---
title: Konfiguracija in odpravljanje težav z SAMLimi zahtevki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901290"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="dd231-102">Konfiguracija in odpravljanje težav z SAMLimi zahtevki</span><span class="sxs-lookup"><span data-stu-id="dd231-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="dd231-103">Če želite konfigurirati in odpraviti SAML terjatve:</span><span class="sxs-lookup"><span data-stu-id="dd231-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="dd231-104">Upoštevajte korake, opisane v [tem članku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) , da konfigurirate terjatev vloge, izdane v SAML žetonu za podjetja.</span><span class="sxs-lookup"><span data-stu-id="dd231-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="dd231-105">Upoštevajte navodila v [tem članku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) , da prilagodite terjatve, ki so bile izdane v SAML žetonu za podjetja.</span><span class="sxs-lookup"><span data-stu-id="dd231-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="dd231-106">Upoštevajte navodila v [tem članku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) , da prilagodite terjatve, ki jih oddajajo žetoni za določen program v najemniku.</span><span class="sxs-lookup"><span data-stu-id="dd231-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="dd231-107">Preberite [Ta članek](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) , da razumete delo z aplikacijami, ki se zavedajo zahtevkov v proxy aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="dd231-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>