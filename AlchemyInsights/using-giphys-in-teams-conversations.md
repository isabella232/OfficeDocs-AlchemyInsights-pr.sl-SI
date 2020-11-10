---
title: Uporaba Giphy v pogovorih Teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982577"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="51a15-102">Uporaba Giphy v pogovorih Teams</span><span class="sxs-lookup"><span data-stu-id="51a15-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="51a15-103">Giphy Access v programu Teams chat je privzeto omogočen.</span><span class="sxs-lookup"><span data-stu-id="51a15-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="51a15-104">Kot skrbnik lahko nadzorujete, ali so Giphy na voljo uporabnikom tako, da [nastavite pravilnik za sporočanje](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) in zagotovite, da je **Uporaba giphy v pogovorih** **vklopljena**.</span><span class="sxs-lookup"><span data-stu-id="51a15-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="51a15-105">Če gif v pogovorih Teams ne deluje po pričakovanjih, preverite:</span><span class="sxs-lookup"><span data-stu-id="51a15-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="51a15-106">[Pravilnik za sporočanje](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora omogočiti giphy.</span><span class="sxs-lookup"><span data-stu-id="51a15-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="51a15-107">Če želite preveriti z uporabo ukazov» cmdlet «PowerShell:</span><span class="sxs-lookup"><span data-stu-id="51a15-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="51a15-108">Preverite, ali lahko [upravljate ekipe z lupino PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="51a15-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="51a15-109">Zaženite ukaz PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) in preverite, ali je **AllowGiphy** nastavljena na **True**.</span><span class="sxs-lookup"><span data-stu-id="51a15-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="51a15-110">Če je argument» **AllowGiphy** «nastavljen na» **FALSE «** , zaženite ta ukaz» [set-CsTeamsMessagingPolicy – Identity «(globalno AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="51a15-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="51a15-111">Če želite omogočiti dostop do URL-ja» Giphy «, morate omogočiti [izbirne povezave](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="51a15-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="51a15-112">Če imate več pravilnikov za sporočanje Teams, konfiguriranih za najemnika, lahko določite identiteto pravilnika, dodeljenega uporabniku, ki je bil uporabnik, z ukazom PowerShell [Get-CsOnlineUser – Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izberite TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="51a15-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
