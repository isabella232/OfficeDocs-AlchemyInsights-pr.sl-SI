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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696974"
---
# <a name="11-call-recording"></a><span data-ttu-id="34358-102">Posnetek klica 1:1</span><span class="sxs-lookup"><span data-stu-id="34358-102">1:1 call recording</span></span>

<span data-ttu-id="34358-103">Če je **gumb Začni** snemanje v klicu 1:1 zatemnjen, morate spremeniti nastavitve pravilnika za uporabnika, na kar to vpliva.</span><span class="sxs-lookup"><span data-stu-id="34358-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="34358-104">Od 31. maja 2021 naprej bomo začeli vsiljevali nov pravilnik Teams za klicanje *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="34358-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="34358-105">Pred to spremembo snemanje klica v 1:1 nadzira pravilnik srečanja *AllowCloudRecording* Teams srečanja.</span><span class="sxs-lookup"><span data-stu-id="34358-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="34358-106">Ta sprememba je zabeležena v objavi v središču za sporočila: [(Posodobljeno) 1:1 Uvod v pravilnik o snemanju klicev.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="34358-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="34358-107">*AllowCloudRecordingForCalls*   Možnost pravilnika za klicanje **$False** nastavljena na privzeto nastavitev.</span><span class="sxs-lookup"><span data-stu-id="34358-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="34358-108">Če želite vsem uporabnikom blokirati snemanje klicev v 1:1, vam ni treba ukrepati.</span><span class="sxs-lookup"><span data-stu-id="34358-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="34358-109">Če želite omogočiti snemanje klicev za vse uporabnike med klici v 1:1, uporabite Teams PowerShell, da zaženete ta ukaz »cmdlet«:</span><span class="sxs-lookup"><span data-stu-id="34358-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="34358-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="34358-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="34358-111">Lahko pa ustvarite nov pravilnik in nastavite **-AllowCloudRecordingForCalls$true** dodelite ta pravilnik uporabnikom. </span><span class="sxs-lookup"><span data-stu-id="34358-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="34358-112">Če želite več informacij, glejte [Kontrolniki pravilnika snemanja klicev v 1:1 so (skoraj!) Tukaj](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="34358-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
