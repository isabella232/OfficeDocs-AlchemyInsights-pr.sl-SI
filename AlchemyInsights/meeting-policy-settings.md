---
title: Nastavitve pravilnika za sestanke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627590"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="835fb-102">Upravljanje pravilnikov za sestanke v storitvi Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="835fb-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="835fb-103">Pravilniki za sestanke se uporabljajo za nadzor funkcij, ki so na voljo za srečanje udeležencev za sestanke, ki so jih načrtovali uporabniki v vaši organizaciji.</span><span class="sxs-lookup"><span data-stu-id="835fb-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="835fb-104">Nekaterih funkcij pravilnikov za sestanke morda ne boste izvajali v skrbniškem središču ekip (ti so označeni z "kmalu" v dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="835fb-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="835fb-105">V tem primeru ali če dobivate napako, kot je» trenutno ne moremo posodobiti pravilnika, ampak poskusite znova pozneje «v skrbniškem središču za Microsoft Teams priporočamo, da uporabite lupino PowerShell za ustvarjanje ali spreminjanje pravilnikov sestankov skupine.</span><span class="sxs-lookup"><span data-stu-id="835fb-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="835fb-106">Če želite več informacij o politikah za sestanke, si oglejte te vire:</span><span class="sxs-lookup"><span data-stu-id="835fb-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="835fb-107">Če želite izvedeti več o ustvarjanju pravilnikov, spreminjanju in dodeljevanju uporabnikov pravilniku, glejte [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="835fb-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="835fb-108">Če želite spremeniti pravilnik s pomočjo ukazov» cmdlet «PowerShell, glejte [pregled skupin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="835fb-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="835fb-109">Za pravilnike za sestanke ekip morate uporabiti [modul Skype za podjetja PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) .</span><span class="sxs-lookup"><span data-stu-id="835fb-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="835fb-110">Preglejte [dokumentacijo» cmdlet «\*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="835fb-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="835fb-111">**Opomba:** Do 24 ur lahko traja, da spremembe pravilnika uveljavljajo za uporabnike.</span><span class="sxs-lookup"><span data-stu-id="835fb-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="835fb-112">Na novo ustvarjene pravilnike morda ne boste mogli takoj spreminjati; Počakajte 4 ure in znova poskusite spremeniti novo ustvarjeno politiko.</span><span class="sxs-lookup"><span data-stu-id="835fb-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="835fb-113">Če imate še vedno težave, poskusite PowerShell.</span><span class="sxs-lookup"><span data-stu-id="835fb-113">If you're still having problems, try PowerShell.</span></span>  