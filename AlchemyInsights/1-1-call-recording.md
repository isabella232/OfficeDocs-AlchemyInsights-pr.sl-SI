---
title: snemanje klicev v 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733865"
---
# <a name="11-call-recording"></a><span data-ttu-id="46a4f-102">snemanje klicev v 1:1</span><span class="sxs-lookup"><span data-stu-id="46a4f-102">1:1 call recording</span></span>

<span data-ttu-id="46a4f-103">Skrbniki morajo zdaj ukrepati, da bodo lahko uporabniki beležili 1:1 klicev.</span><span class="sxs-lookup"><span data-stu-id="46a4f-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="46a4f-104">Začetek april 12, 2021, bomo začeli uveljaviti novo Teams Calling Policy option *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="46a4f-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="46a4f-105">Trenutno so zmogljivosti snemanja klicev v 1:1 nadzorovane z možnostjo *AllowCloudRecording* v pravilnikih za srečanje ekip.</span><span class="sxs-lookup"><span data-stu-id="46a4f-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="46a4f-106">Če lahko vaši uporabniki snemajo sestanke v Teams, bodo morda snemali tudi 1:1 klicev.</span><span class="sxs-lookup"><span data-stu-id="46a4f-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="46a4f-107">Če želite blokirati vse uporabnike iz snemanja 1:1 klicev, vam ni treba izvesti nobenega dejanja.</span><span class="sxs-lookup"><span data-stu-id="46a4f-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="46a4f-108">Možnost» *AllowCloudRecordingForCalls* Calling pravilnik «bo privzeto $FALSE.</span><span class="sxs-lookup"><span data-stu-id="46a4f-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="46a4f-109">Ta sprememba je dokumentirana v tej objavi v središču za sporočila: [(posodobljeno) 1:1 vnos pravilnika o snemanju](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) , da nastavite možnost pravilnika za [klicanje ekip](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="46a4f-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="46a4f-110">**Če želite omogočiti snemanje klicev v 1:1 klici:** Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="46a4f-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="46a4f-111">**Če želite onemogočiti snemanje klicev v 1:1 klici:** Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $FALSE</span><span class="sxs-lookup"><span data-stu-id="46a4f-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

