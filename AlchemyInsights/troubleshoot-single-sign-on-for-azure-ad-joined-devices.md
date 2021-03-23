---
title: Odpravljanje težav z enim samim vpisom za naprave v storitvi Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037333"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="854f8-102">Odpravljanje težav z enim samim vpisom za naprave v storitvi Azure AD</span><span class="sxs-lookup"><span data-stu-id="854f8-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="854f8-103">Če imate okolje Active Directory (AD) na mestu uporabe in se želite pridružiti računalnikom, povezanim z domeno OGLASa, v storitvi Azure AD, lahko to dosežete tako, da izvedete hibridno pridružitev za oglase.</span><span class="sxs-lookup"><span data-stu-id="854f8-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="854f8-104">[Kako: načrtovati vaš hibridni postopek združevanja v storitvi Hybrid Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vam ponuja povezane korake za izvajanje hibridnega združevanja oglasov v okolju.</span><span class="sxs-lookup"><span data-stu-id="854f8-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="854f8-105">Če želite več informacij, glejte [Konfiguracija naprav v storitvi AZURE ad JOIN za Single-Sign na mestu uporabe v storitvi Windows hello za podjetja](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="854f8-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="854f8-106">**Težave primarnega osveževanja (PRT)**</span><span class="sxs-lookup"><span data-stu-id="854f8-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="854f8-107">Primarni žeton za osveževanje (PRT) je ključni artefakt za preverjanje pristnosti storitve Azure AD v sistemih Windows 10, Windows Server 2016 in novejših različicah, iOS in naprave s sistemom Android.</span><span class="sxs-lookup"><span data-stu-id="854f8-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="854f8-108">Gre za spletni žeton JSON (JWT), ki je posebej izdan za posrednike za žetone Microsoft First Party, da omogoči enotno prijavo (SSO) med programi, ki so uporabljeni v teh napravah.</span><span class="sxs-lookup"><span data-stu-id="854f8-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="854f8-109">Če želite več informacij o tem, kako je PRT izdan, uporabljen in zaščiten v napravah s sistemom Windows 10, glejte [Kaj je primarni žeton za osveževanje?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="854f8-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="854f8-110">**WamDefaultSet: da in AzureADPrt: da**</span><span class="sxs-lookup"><span data-stu-id="854f8-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="854f8-111">V teh poljih je navedeno, ali se je uporabnik uspešno potrdil na Azure AD, ko se je prijavljal v napravo.</span><span class="sxs-lookup"><span data-stu-id="854f8-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="854f8-112">Če **vrednosti niso:**</span><span class="sxs-lookup"><span data-stu-id="854f8-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="854f8-113">Napačen ključ za shranjevanje v modulu zaupanja TPM, ki je povezan z napravo ob registraciji (preverite KeySignTest med izvajanjem povišane vrednosti)</span><span class="sxs-lookup"><span data-stu-id="854f8-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="854f8-114">Nadomestni ID za prijavo</span><span class="sxs-lookup"><span data-stu-id="854f8-114">Alternate Login ID</span></span>
- <span data-ttu-id="854f8-115">Proxyja HTTP ni bilo mogoče najti</span><span class="sxs-lookup"><span data-stu-id="854f8-115">HTTP Proxy not found</span></span>

<span data-ttu-id="854f8-116">Če želite odpraviti težave z ukazom» dsregcmd «, glejte [stanje SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="854f8-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
