---
title: Posnetek klica 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702106"
---
# <a name="11-call-recording"></a><span data-ttu-id="404e8-102">Posnetek klica 1:1</span><span class="sxs-lookup"><span data-stu-id="404e8-102">1:1 call recording</span></span>

<span data-ttu-id="404e8-103">Če je **gumb Začni** snemanje v klicu 1:1 zatemnjen, morate spremeniti nastavitve pravilnika za uporabnika, na kar to vpliva.</span><span class="sxs-lookup"><span data-stu-id="404e8-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="404e8-104">Če želite preveriti nastavitev pravilnika, zaženite diagnostično diagnostiko za ega uporabnika, tako da zgoraj vnesete **Diag: Teams 1:1 Snemanje** klica zgoraj.</span><span class="sxs-lookup"><span data-stu-id="404e8-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="404e8-105">Od 31. maja 2021 naprej bomo začeli vsiljevali nov pravilnik Teams za klicanje *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="404e8-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="404e8-106">Pred to spremembo snemanje klica v 1:1 nadzira pravilnik srečanja *AllowCloudRecording* Teams srečanja.</span><span class="sxs-lookup"><span data-stu-id="404e8-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="404e8-107">Ta sprememba je zabeležena v objavi v središču za sporočila: [(Posodobljeno) 1:1 Uvod v pravilnik o snemanju klicev.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="404e8-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="404e8-108">*AllowCloudRecordingForCalls*   Možnost pravilnika za klicanje **$False** nastavljena na privzeto nastavitev.</span><span class="sxs-lookup"><span data-stu-id="404e8-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="404e8-109">Če želite vsem uporabnikom blokirati snemanje klicev v 1:1, vam ni treba ukrepati.</span><span class="sxs-lookup"><span data-stu-id="404e8-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="404e8-110">Če želite omogočiti snemanje klicev za vse uporabnike med klici v 1:1, [uporabite Teams PowerShell,](/microsoftteams/teams-powershell-install) da zaženete ta ukaz »cmdlet«:</span><span class="sxs-lookup"><span data-stu-id="404e8-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="404e8-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="404e8-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="404e8-112">Lahko pa ustvarite nov pravilnik in nastavite **-AllowCloudRecordingForCalls$true** dodelite ta pravilnik uporabnikom. </span><span class="sxs-lookup"><span data-stu-id="404e8-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="404e8-113">Če želite več informacij, glejte [Kontrolniki pravilnika snemanja klicev v 1:1 so (skoraj!) Tukaj](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="404e8-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
