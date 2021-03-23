---
title: Povezava do ZVOČNIh obvestil
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037236"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="3ba9d-102">Povezava do ZVOČNIh obvestil</span><span class="sxs-lookup"><span data-stu-id="3ba9d-102">Notification AAD Connect</span></span>

- <span data-ttu-id="3ba9d-103">Zagotovite, da imate dovoljenje za izvedbo operacije.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="3ba9d-104">Globalni skrbniki imajo privzeto dostop do njih.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-104">Global Admins have access by default.</span></span> <span data-ttu-id="3ba9d-105">Poleg tega lahko uporabite [nadzor dostopa](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , ki temelji na vlogi, če želite dodeliti dovoljenje za registracijo plačniku.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="3ba9d-106">Zagotovite, da so zahtevane končne točke omogočene in niso blokirane zaradi požarnega zidu.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="3ba9d-107">Če želite več informacij, glejte [zahteve](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="3ba9d-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="3ba9d-108">Registracija ni mogoča zaradi odhodne komunikacije, ki jo je treba pregledati prek omrežja SSL.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="3ba9d-109">Preverite, ali ste preverili nastavitve obvestila za Azure AD Connect Health in preverite nastavitev.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="3ba9d-110">Če želite izvedeti, kako konfigurirate nastavitve obvestila za obvestila o zdravju Azure AD Connect, si oglejte ta [vodnik](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="3ba9d-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="3ba9d-111">Če želite izvedeti več o poročilu o sinhronizaciji ZVOČNIh povezav in kako jo prenesti, glejte [poročilo o sinhronizaciji ravni predmeta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="3ba9d-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="3ba9d-112">Če želite odpraviti težave z zdravstvenimi opozorili, preberite [navodila za odpravljanje težav z navodili za zvočno povezavo](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) in za pogosto zastavljena vprašanja glejte [pogosta vprašanja o zdravstveni namestitvi](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="3ba9d-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
