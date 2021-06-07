---
title: Omogočanje Teams Webinars
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794039"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="95b6d-102">Omogočanje Teams Webinars</span><span class="sxs-lookup"><span data-stu-id="95b6d-102">Enable Teams Webinars</span></span>

<span data-ttu-id="95b6d-103">Spletni seminarji so omogočeni privzeto.</span><span class="sxs-lookup"><span data-stu-id="95b6d-103">Webinars are enabled by default.</span></span> <span data-ttu-id="95b6d-104">Upravljate lahko, kdo lahko načrtuje in registrira za Teams webinars, tako da Teams ukazi powershell.</span><span class="sxs-lookup"><span data-stu-id="95b6d-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="95b6d-105">Vsi uporabniki, ki lahko ustvarijo srečanje, lahko prav tako ustvarijo srečanje spletnega seminarja.</span><span class="sxs-lookup"><span data-stu-id="95b6d-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="95b6d-106">Če želite upravljati, kdo lahko načrtuje Teams Webinars, uporabite *AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="95b6d-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="95b6d-107">Privzeto je *možnost WhoCanRegister* omogočena in nastavljena na **Vsi.**</span><span class="sxs-lookup"><span data-stu-id="95b6d-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="95b6d-108">Če želite izklopiti registracijo srečanja, nastavite *AllowMeetingRegistration* na **False.**</span><span class="sxs-lookup"><span data-stu-id="95b6d-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="95b6d-109">Če želite spremeniti te nastavitve, morate namestiti [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="95b6d-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="95b6d-110">Pravilniki srečanja se izvajajo tudi za spletne Teams spletnih seminarjih.</span><span class="sxs-lookup"><span data-stu-id="95b6d-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="95b6d-111">Če je na primer anonimna pridružitev v nastavitvah srečanja izklopljena, se anonimni uporabniki ne morejo pridružiti spletnim seminarjem.</span><span class="sxs-lookup"><span data-stu-id="95b6d-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="95b6d-112">Če želite izvedeti več o konfiguraciji, kdo se lahko prijavi za spletne seminarje, glejte [Konfiguriranje, kdo se lahko prijavi za spletne seminarje.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="95b6d-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="95b6d-113">Če želite več informacij o nastavitvah za Microsoftove sezname, glejte [Nadzor nastavitev za Microsoftove sezname.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="95b6d-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>