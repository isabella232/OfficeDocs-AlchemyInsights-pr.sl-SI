---
title: Nastavitve pravilnika srečanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704622"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="0bc68-102">Upravljanje pravilnikov za srečanje v aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0bc68-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="0bc68-103">**Opomba: Če želite, da bodo spremembe pravilnika veljale za uporabnike, lahko traja do 24 ur.**</span><span class="sxs-lookup"><span data-stu-id="0bc68-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="0bc68-104">Morda ne boste mogli takoj spreminjati novih pravilnikov; Počakajte 4 ure in poskusite znova spremeniti novo ustvarjen pravilnik.</span><span class="sxs-lookup"><span data-stu-id="0bc68-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="0bc68-105">Pravilniki o srečanju se uporabljajo za nadzor funkcij, ki so na voljo za srečanja udeležencev za srečanja, ki jih načrtujejo uporabniki v vaši organizaciji.</span><span class="sxs-lookup"><span data-stu-id="0bc68-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="0bc68-106">Nekatere funkcije pravilnikov srečanja morda ne bodo uveljavljene v skrbniškem središču za Teams (ti so označeni» kmalu na voljo «v dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="0bc68-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="0bc68-107">V tem primeru ali če se prikaže sporočilo o napaki, kot je» trenutno ne moremo posodobiti pravilnika, vendar poskusite znova pozneje «v skrbniškem središču za Microsoft Teams, vam priporočamo, da uporabite PowerShell za ustvarjanje ali spreminjanje pravilnikov skupine za srečanje.</span><span class="sxs-lookup"><span data-stu-id="0bc68-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="0bc68-108">Če želite več informacij o pravilnikih za srečanje, si oglejte te vire:</span><span class="sxs-lookup"><span data-stu-id="0bc68-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="0bc68-109">Če želite izvedeti več o ustvarjanju pravilnikov, spreminjanju in dodeljevanju uporabnikov v pravilnik, glejte [upravljanje pravilnikov za srečanje v aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="0bc68-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="0bc68-110">Če želite spremeniti pravilnike z ukazi» cmdlet «PowerShell, glejte [pregled skupine PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="0bc68-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="0bc68-111">Za pravilnike o srečanju Teams morate uporabiti [modul za Skype za podjetja PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) .</span><span class="sxs-lookup"><span data-stu-id="0bc68-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="0bc68-112">Če želite več informacij, si oglejte [dokumentacijo» cmdlet «za CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="0bc68-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

