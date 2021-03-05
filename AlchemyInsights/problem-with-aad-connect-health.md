---
title: Težave s ZVOČNO povezavo za zdravje
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483120"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="45e8c-102">Težave s ZVOČNO povezavo za zdravje</span><span class="sxs-lookup"><span data-stu-id="45e8c-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="45e8c-103">Zagotovite, da imate dovoljenje za izvedbo operacije.</span><span class="sxs-lookup"><span data-stu-id="45e8c-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="45e8c-104">Globalni skrbniki imajo privzeto dostop do njih.</span><span class="sxs-lookup"><span data-stu-id="45e8c-104">Global Admins have access by default.</span></span> <span data-ttu-id="45e8c-105">Poleg tega lahko uporabite [nadzor dostopa](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , ki temelji na vlogi, če želite dodeliti dovoljenje za registracijo plačniku.</span><span class="sxs-lookup"><span data-stu-id="45e8c-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="45e8c-106">Zagotovite, da so zahtevane končne točke omogočene in niso blokirane zaradi požarnega zidu.</span><span class="sxs-lookup"><span data-stu-id="45e8c-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="45e8c-107">Če želite več informacij, glejte [zahteve](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="45e8c-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="45e8c-108">Registracija ni mogoča zaradi odhodne komunikacije, ki jo je treba pregledati prek omrežja SSL.</span><span class="sxs-lookup"><span data-stu-id="45e8c-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="45e8c-109">Preverite, ali ste preverili nastavitve obveščanja za povezavo z zdravjem za Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="45e8c-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="45e8c-110">Oglejte si nastavitev.</span><span class="sxs-lookup"><span data-stu-id="45e8c-110">Please review your setting.</span></span> <span data-ttu-id="45e8c-111">S tem [vodnikom](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) lahko razumete, kako konfigurirate nastavitve obvestila za obvestila o zdravju v storitvi Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="45e8c-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="45e8c-112">Če želite izvedeti več o poročilu o sinhronizaciji ZVOČNIh povezav in kako jo prenesti, glejte [poročilo o sinhronizaciji ravni predmeta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="45e8c-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="45e8c-113">Če želite odpraviti težave z zdravstvenimi opozorili, si oglejte [navodila za odpravljanje težav s povezovanjem zdravstvenih podatkov](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) in za pogosta vprašanja o [pogostosti težav s povezovanjem zdravja](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="45e8c-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
