---
title: Nastavitve pravilnika srečanja
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825459"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="a15d1-102">Upravljanje pravilnikov za srečanja v aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a15d1-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="a15d1-103">**Opomba: Traja lahko do 24 ur, preden spremembe pravilnika začne veljati za uporabnike.**</span><span class="sxs-lookup"><span data-stu-id="a15d1-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="a15d1-104">Morda ne boste mogli takoj spreminjati novo ustvarjenih pravilnikov; počakajte 4 ure in poskusite znova spremeniti novo ustvarjeni pravilnik.</span><span class="sxs-lookup"><span data-stu-id="a15d1-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="a15d1-105">S pravilniki srečanja nadzorujete funkcije, ki so na voljo udeležencem srečanja za srečanja, ki jih načrtujejo uporabniki v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="a15d1-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="a15d1-106">Nekatere funkcije pravilnikov srečanja morda še ne bodo na voljo v skrbniškem središču za Teams (v dokumentaciji so označene kot »kmalu na voljo«).</span><span class="sxs-lookup"><span data-stu-id="a15d1-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="a15d1-107">Če se v tem primeru prikaže napaka, kot je »Pravilnika trenutno ni mogoče posodobiti, lahko pa ga poskusite znova pozneje« v skrbniškem središču za Microsoft Teams, priporočamo, da uporabite PowerShell za ustvarjanje ali spreminjanje pravilnikov za srečanja v storitvi Teams.</span><span class="sxs-lookup"><span data-stu-id="a15d1-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="a15d1-108">Če želite več informacij o pravilnikih srečanja, glejte te vire:</span><span class="sxs-lookup"><span data-stu-id="a15d1-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="a15d1-109">Če želite izvedeti več o ustvarjanju pravilnikov, spremembami in dodeljevanju uporabnikov pravilniku, glejte [Upravljanje pravilnikov o srečanju v teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="a15d1-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="a15d1-110">Če želite spremeniti pravilnik z ukazi »cmdlet« lupine PowerShell, glejte [Pregled storitve PowerShell za Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="a15d1-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="a15d1-111">Uporabiti morate modul [PowerShell za Skype za podjetja za pravilnike](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) srečanja v storitvi Teams.</span><span class="sxs-lookup"><span data-stu-id="a15d1-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="a15d1-112">Za več informacij preglejte dokumentacijo z ukazi [»cmdlet« \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="a15d1-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

