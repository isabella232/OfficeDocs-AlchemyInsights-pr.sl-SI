---
title: Single-Sign v napravah, ki so pridružene imeniku Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405661"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="7586e-102">Enotna prijava za naprave, ki so pridružene imeniku Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7586e-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="7586e-103">Če imate okolje imenika Active Directory (AD) na mestu uporabe in želite svoje računalnike, pridružene domeni AD, pridružiti imeniku Azure AD, lahko to dosežete tako, da izvedete hibridno pridružitev imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7586e-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="7586e-104">[Kako: Načrtujte hibridno združevanje](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) imenika Azure Active Directory vam ponuja sorodne korake za izvedbo hibridne pridružine storitve Azure AD v vašem okolju.</span><span class="sxs-lookup"><span data-stu-id="7586e-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="7586e-105">Konfiguracija naprav, ki so pridružene imeniku Azure AD, za Single-Sign na mestu uporabe: uporaba funkcije Windows Hello za podjetja</span><span class="sxs-lookup"><span data-stu-id="7586e-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="7586e-106">**Težave s primarnim žetonom za osveževanje (PRT)** Primarni žeton za osveževanje (PRT) je ključni element preverjanja pristnosti imenika Azure AD v sistemih Windows 10, Windows Server 2016 in novejših različicah ter napravah s sistemom iOS in Android.</span><span class="sxs-lookup"><span data-stu-id="7586e-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="7586e-107">Gre za žeton JSON Web Token (JWT), ki je posebej izdan Microsoftovim žetonom prve stranke, da omogoči enotno prijavo (SSO) v programih, ki se uporabljajo v teh napravah.</span><span class="sxs-lookup"><span data-stu-id="7586e-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="7586e-108">[V oknu Kaj je primarni](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)žeton za osveževanje? bomo objavili podrobnosti o tem, kako se izda, uporablja in zaščiti PRT v napravah s sistemom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7586e-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="7586e-109">**WamDefaultSet: DA in AzureADPrt: DA** Ta polja označujejo, ali je uporabnik ob vpisu v napravo uspešno preverjal pristnost imenika Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7586e-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="7586e-110">Če so vrednosti **»NO),** lahko zapadejo:</span><span class="sxs-lookup"><span data-stu-id="7586e-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="7586e-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span><span class="sxs-lookup"><span data-stu-id="7586e-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="7586e-112">Nadomestni ID za prijavo</span><span class="sxs-lookup"><span data-stu-id="7586e-112">Alternate Login ID</span></span>
- <span data-ttu-id="7586e-113">STREŽNIKA HTTP Proxy ni bilo mogoče najti</span><span class="sxs-lookup"><span data-stu-id="7586e-113">HTTP Proxy not found</span></span>

<span data-ttu-id="7586e-114">Odpravljanje težav z uporabo ukaza dsregcmd – [stanje SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="7586e-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
