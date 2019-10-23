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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637793"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="0fb3f-102">Nadzor nastavitev lobistov in raven udeležbe</span><span class="sxs-lookup"><span data-stu-id="0fb3f-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="0fb3f-103">Če želite dovoliti vsem, vključno z dial-in, zunanjimi in anonimnimi Uporabniki, da zaobide preddverje, lahko uporabite PowerShell za to.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="0fb3f-104">Tukaj je primer spreminjanja globalne politike srečanja za vašo organizacijo:</span><span class="sxs-lookup"><span data-stu-id="0fb3f-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="0fb3f-105">Ta ukaz» cmdlet «trenutno zahteva uporabo modula Skype za podjetja PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="0fb3f-106">Če želite dobiti nastavitev za uporabo tega ukaza» cmdlet «, si oglejte upravljanje pravilnikov prek lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="0fb3f-107">Nastavite lahko novo politiko, ki jo boste nato morali uporabiti za uporabnike.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="0fb3f-108">Če spremenite globalno politiko, bo samodejno veljala za uporabnike.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="0fb3f-109">Za vsako spremembo pravilnika morate počakati vsaj 4 ure in do 24 ur, da se bodo pravilniki uveljavili.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="0fb3f-110">Bodite prepričani, da pregleda dokumentacijo spodaj, preden te spremembe razumeti, kaj to omogoča.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="0fb3f-111">Razumevanje ekip, ki izpolnjujejo nadzorne politike lobistov</span><span class="sxs-lookup"><span data-stu-id="0fb3f-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="0fb3f-112">[Samodejno priznam](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , da so ljudje po-organizator politike, ki nadzoruje, ali se ljudje pridružijo srečanju neposredno ali čakati v preddverju, dokler jih ne sprejme overjeni uporabnik.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="0fb3f-113">[Omogočanje anonimnih oseb, da začnejo sestanek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik za organizatorja, ki nadzoruje, ali se lahko anonimni ljudje, vključno z B2B in federativne Uporabniki, pridružijo sestanku uporabnika brez overjenega uporabnika iz organizacije v navzočnosti.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="0fb3f-114">[Omogučiti sončna ura-v uporabnik v bypass preddverje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**bodoč zgodaj**) je a po-organizator zvitost to kontrolni aparati ali narod kdo sončna ura v z telefon združiti sestanek naravnost ali čakati v preddverje če ne **automatically priznajte narod** postavljanje.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="0fb3f-115">[Dovolite organizatorjem, da preglasijo nastavitve v preddverju](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**) je pravilnik za organizatorja, ki nadzira, ali lahko organizator srečanja preglasi nastavitve v preddverju, ki jih admin Nastavi v **samodejno prizna ljudi** in **Dovoli klicanje uporabnikom, da obidejo preddverje** , ko načrtujete nov sestanek.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="0fb3f-116">**Opomba:** Preberite [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za sestanke programa Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="0fb3f-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
