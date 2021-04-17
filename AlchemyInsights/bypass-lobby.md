---
title: Obhodna čakalnica
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820050"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="79761-102">Nadzor nastavitev čakalnice in raven sodelovanja v teams</span><span class="sxs-lookup"><span data-stu-id="79761-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="79761-103">Če želite vsem, vključno s klicnimi, zunanjimi in anonimnimi uporabniki, dovoliti, da preskočijo čakalnico **,** za dokončanje tega opravila uporabite PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79761-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="79761-104">Spodaj je primer spreminjanja pravilnika globalnega srečanja za vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="79761-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="79761-105">Ta ukaz »cmdlet« trenutno zahteva uporabo modula PowerShell za Skype za podjetja.</span><span class="sxs-lookup"><span data-stu-id="79761-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="79761-106">Če želite nastaviti uporabo tega ukaza »cmdlet« , si oglejte [Upravljanje pravilnikov prek lupine PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="79761-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="79761-107">Ko nastavite pravilnik, ga morate uporabiti za uporabnike. če ste spremenili globalni pravilnik, pa bo samodejno veljal za uporabnike.</span><span class="sxs-lookup"><span data-stu-id="79761-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="79761-108">Če želite spremeniti pravilnik, morate počakati vsaj 4 ure do **24** ur, da bodo pravilniki veljati.</span><span class="sxs-lookup"><span data-stu-id="79761-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="79761-109">Preden spremenite dokument, preberite spodnjo dokumentacijo, da boste natančno razumeli, kaj to omogoča.</span><span class="sxs-lookup"><span data-stu-id="79761-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="79761-110">Razumevanje kontrolnikov pravilnika čakalnice za srečanja v teams</span><span class="sxs-lookup"><span data-stu-id="79761-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="79761-111">Te nastavitve nadzirajo, kateri udeleženci srečanja počakajo v čakalnici, preden so sprejeti v srečanje, in raven sodelovanja, ki jim je dovoljena v srečanju.</span><span class="sxs-lookup"><span data-stu-id="79761-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="79761-112">S storitvijo PowerShell lahko posodobite nastavitve pravilnika srečanja, ki še niso bile implementirane (v skrbniškem središču za Teams so označene z »kmalu na voljo«).</span><span class="sxs-lookup"><span data-stu-id="79761-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="79761-113">Glejte spodaj za primer ukaza »cmdlet« lupine PowerShell, ki vsem uporabnikom omogoča, da preskočijo čakalnico.</span><span class="sxs-lookup"><span data-stu-id="79761-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="79761-114">[Samodejno sprejem oseb je](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) pravilnik na organizatorja, ki nadzira, ali se osebe pridružijo srečanju neposredno ali pa počakajo v čakalnici, dokler jih ne sprejmejo uporabnik s preverjeno pristnostjo.</span><span class="sxs-lookup"><span data-stu-id="79761-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="79761-115">[Anonimnim](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ljudem dovoli začetek srečanja je pravilnik na organizatorja, ki nadzira, ali se lahko anonimne osebe, vključno z B2B in zunanji uporabniki, pridružijo srečanju uporabnika brez preverjenega uporabnika iz organizacije, ki se udeleži.</span><span class="sxs-lookup"><span data-stu-id="79761-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="79761-116">[Dovoli,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) da klicni uporabniki preskočijo čakalnico **(** kmalu na voljo ) je pravilnik na organizatorja, ki nadzira, ali se osebe, ki so se srečanju neposredno pridružile s klicem po telefonu, ali pa počakajo v čakalnici ne glede na nastavitev Samodejno dovoli **dostop** oseb.</span><span class="sxs-lookup"><span data-stu-id="79761-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="79761-117">[Dovoli](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) organizatorjem, da preglasijo nastavitve čakalnice **(** kmalu na voljo ) je pravilnik na  organizatorja, ki nadzoruje, ali lahko organizator srečanja preglasi nastavitve čakalnice, ki jih je nastavil skrbnik v možnosti Samodejno dovoli sprejem oseb **in** Dovoli, da klicni uporabniki preskočijo čakalnico, ko načrtujejo novo srečanje.</span><span class="sxs-lookup"><span data-stu-id="79761-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="79761-118">**Opomba:** Celoten [pregled pravilnikov za srečanja v aplikaciji](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) Microsoft Teams je na voljo v članku Upravljanje pravilnikov za srečanja v aplikaciji Teams.</span><span class="sxs-lookup"><span data-stu-id="79761-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
