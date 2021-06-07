---
title: Upravljanje registracije spletnega seminarja
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794146"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="6abd0-102">Upravljanje registracije spletnega seminarja</span><span class="sxs-lookup"><span data-stu-id="6abd0-102">Manage webinar registration</span></span>

<span data-ttu-id="6abd0-103">Upravljate, kdo se lahko prijavi za Teams Webinars, tako da Teams ukazi powershell.</span><span class="sxs-lookup"><span data-stu-id="6abd0-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="6abd0-104">Če želite Teams Powershell, glejte [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="6abd0-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="6abd0-105">Privzeto je *možnost WhoCanRegister* omogočena in nastavljena na **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="6abd0-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="6abd0-106">Če želite vsem, vključno z anonimnimi uporabniki, dovoliti registracijo, morate pravilnik srečanja nastaviti na **»Vsi«** z ukazom Powershell:</span><span class="sxs-lookup"><span data-stu-id="6abd0-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="6abd0-107">**Opomba: Če** je v nastavitvah srečanja anonimna pridružitev izklopljena, se anonimni uporabniki ne morejo pridružiti spletnim seminarjem.</span><span class="sxs-lookup"><span data-stu-id="6abd0-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="6abd0-108">Če želite izvedeti več in omogočiti to nastavitev, glejte [Upravljanje nastavitev srečanja v Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6abd0-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="6abd0-109">Če želite izklopiti registracijo srečanja, nastavite *AllowMeetingRegistration* na **False.**</span><span class="sxs-lookup"><span data-stu-id="6abd0-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="6abd0-110">Če želite izvedeti več o konfiguraciji, kdo se lahko prijavi za spletne seminarje, glejte [Konfiguriranje, kdo se lahko prijavi za spletne seminarje.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="6abd0-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="6abd0-111">Če želite več informacij o nastavitvah za Microsoftove sezname, glejte [Nadzor nastavitev za Microsoftove sezname.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="6abd0-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
