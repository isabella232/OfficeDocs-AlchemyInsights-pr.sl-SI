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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376837"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="8da3b-102">Nadzor nastavitev lobistov in raven udeležbe</span><span class="sxs-lookup"><span data-stu-id="8da3b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="8da3b-103">Te nastavitve nadzorujejo, kateri Udeleženci sestanka čakajo v preddverju, preden so sprejeti na sestanek, in raven udeležbe, ki so jim dovoljene na sestanku.</span><span class="sxs-lookup"><span data-stu-id="8da3b-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="8da3b-104">Z lupino PowerShell lahko posodobite nastavitve pravilnika za sestanke, ki še niso bile izvedene (z oznako» kmalu «) v skrbniškem središču ekip.</span><span class="sxs-lookup"><span data-stu-id="8da3b-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="8da3b-105">Glej spodaj za primer cmdlet PowerShell, ki omogoča vsem uporabnikom, da zaobide lobby.</span><span class="sxs-lookup"><span data-stu-id="8da3b-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="8da3b-106">[Samodejno priznam](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , da so ljudje po-organizator politike, ki nadzoruje, ali se ljudje pridružijo srečanju neposredno ali čakati v preddverju, dokler jih ne sprejme overjeni uporabnik.</span><span class="sxs-lookup"><span data-stu-id="8da3b-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="8da3b-107">[Omogočanje anonimnih oseb, da začnejo sestanek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik za organizatorja, ki nadzoruje, ali se lahko anonimni ljudje, vključno z B2B in federativne Uporabniki, pridružijo sestanku uporabnika brez overjenega uporabnika iz organizacije v navzočnosti.</span><span class="sxs-lookup"><span data-stu-id="8da3b-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="8da3b-108">[Omogučiti sončna ura-v uporabnik v bypass preddverje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**bodoč zgodaj**) je a po-organizator zvitost to kontrolni aparati ali narod kdo sončna ura v z telefon združiti sestanek naravnost ali čakati v preddverje če ne **automatically priznajte narod** postavljanje.</span><span class="sxs-lookup"><span data-stu-id="8da3b-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="8da3b-109">[Dovolite organizatorjem, da preglasijo nastavitve v preddverju](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**) je pravilnik za organizatorja, ki nadzira, ali lahko organizator srečanja preglasi nastavitve v preddverju, ki jih admin Nastavi v **samodejno prizna ljudi** in **Dovoli klicanje uporabnikom, da obidejo preddverje** , ko načrtujete nov sestanek.</span><span class="sxs-lookup"><span data-stu-id="8da3b-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="8da3b-110">**Opomba:** Preberite [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za sestanke programa Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="8da3b-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="8da3b-111">**Primer lupine**</span><span class="sxs-lookup"><span data-stu-id="8da3b-111">**PowerShell example**</span></span>

<span data-ttu-id="8da3b-112">Če želite vsem, vključno z zunanjimi ali anonimnimi Uporabniki, dovoliti, da zaobide čakalnico, lahko za dokončanje te naloge uporabite tudi lupino PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8da3b-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="8da3b-113">Tukaj je primer spreminjanja globalne politike srečanja za vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="8da3b-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="8da3b-114">(Bodite prepričani, da pregleda dokumentacijo zgoraj, preden te spremembe razumeti, kaj to omogoča.)</span><span class="sxs-lookup"><span data-stu-id="8da3b-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="8da3b-115">Set-CsTeamsMeetingPolicy-identiteta Global-Autovključitvi Tedusers "vsakdo"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="8da3b-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="8da3b-116">Če želite več informacij, glejte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="8da3b-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
