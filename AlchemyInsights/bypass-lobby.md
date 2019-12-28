---
title: Obvoznica v preddverju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889098"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="bf04a-102">Nadzor nastavitev lobistov in raven udeležbe v ekipah</span><span class="sxs-lookup"><span data-stu-id="bf04a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="bf04a-103">Če želite omogočiti vsem, vključno z dial-in, zunanjimi in anonimnimi Uporabniki, da **zaobide preddverje**, uporabite PowerShell za dokončanje te naloge.</span><span class="sxs-lookup"><span data-stu-id="bf04a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="bf04a-104">Tukaj je primer spreminjanja globalne politike srečanja za vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="bf04a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="bf04a-105">Ta ukaz» cmdlet «trenutno zahteva uporabo modula Skype za podjetja PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bf04a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="bf04a-106">Če želite nastaviti uporabo tega ukaza» cmdlet «, preverite [pravilnike upravljanja prek lupine PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="bf04a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="bf04a-107">Ko nastavite pravilnik, ga morate uporabiti za uporabnike; ali, če ste spremenili globalno politiko, se bo samodejno uporabljal za uporabnike.</span><span class="sxs-lookup"><span data-stu-id="bf04a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="bf04a-108">Za vsako spremembo pravilnika morate počakati vsaj **4 ure do 24 ur** , da se bodo pravilniki uveljavili.</span><span class="sxs-lookup"><span data-stu-id="bf04a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="bf04a-109">Bodite prepričani, da pregleda dokumentacijo spodaj, preden te spremembe razumeti, kaj to omogoča.</span><span class="sxs-lookup"><span data-stu-id="bf04a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="bf04a-110">Razumevanje ekip, ki izpolnjujejo nadzorne politike lobistov</span><span class="sxs-lookup"><span data-stu-id="bf04a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="bf04a-111">Te nastavitve nadzorujejo, kateri Udeleženci sestanka čakajo v preddverju, preden so sprejeti na sestanek, in raven udeležbe, ki so jim dovoljene na sestanku.</span><span class="sxs-lookup"><span data-stu-id="bf04a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="bf04a-112">Z lupino PowerShell lahko posodobite nastavitve pravilnika za sestanke, ki še niso bile izvedene (z oznako» kmalu «) v skrbniškem središču ekip.</span><span class="sxs-lookup"><span data-stu-id="bf04a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="bf04a-113">Glej spodaj za primer cmdlet PowerShell, ki omogoča vsem uporabnikom, da zaobide lobby.</span><span class="sxs-lookup"><span data-stu-id="bf04a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="bf04a-114">[Samodejno priznam](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , da so ljudje po-organizator politike, ki nadzoruje, ali se ljudje pridružijo srečanju neposredno ali čakati v preddverju, dokler jih ne sprejme overjeni uporabnik.</span><span class="sxs-lookup"><span data-stu-id="bf04a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="bf04a-115">[Omogočanje anonimnih oseb, da začnejo sestanek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik za organizatorja, ki nadzoruje, ali se lahko anonimni ljudje, vključno z B2B in federativne Uporabniki, pridružijo sestanku uporabnika brez overjenega uporabnika iz organizacije v navzočnosti.</span><span class="sxs-lookup"><span data-stu-id="bf04a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="bf04a-116">[Omogučiti sončna ura-v uporabnik v bypass preddverje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**bodoč zgodaj**) je a po-organizator zvitost to kontrolni aparati ali narod kdo sončna ura v z telefon združiti sestanek naravnost ali čakati v preddverje če ne **automatically priznajte narod** postavljanje.</span><span class="sxs-lookup"><span data-stu-id="bf04a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="bf04a-117">[Dovolite organizatorjem, da preglasijo nastavitve lobistov](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**) je pravilnik za organizatorja, ki nadzira, ali lahko organizator srečanja preglasi nastavitve v preddverju, ki jih skrbnik Nastavi v **samodejno Sprejmi ljudi** in **Dovoli uporabnikom klicanja, da obidejo čakalnico** , ko razporeja novo sejo.</span><span class="sxs-lookup"><span data-stu-id="bf04a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="bf04a-118">**Opomba:** Preberite [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za sestanke programa Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="bf04a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
