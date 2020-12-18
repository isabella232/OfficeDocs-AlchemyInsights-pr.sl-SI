---
title: Napake sinhronizacije samodejnega vpisa v napravo Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714975"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="3160a-102">Napake sinhronizacije samodejnega vpisa v napravo Apple</span><span class="sxs-lookup"><span data-stu-id="3160a-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="3160a-103">» Zaznali smo, da imate enega ali več žetonov ADE/DEP, ki so v stanju napake.</span><span class="sxs-lookup"><span data-stu-id="3160a-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="3160a-104">Dokler stanje napake ni razrešeno za vsak prizadeti žeton, funkcija ADE ne bo delovala enako kot».</span><span class="sxs-lookup"><span data-stu-id="3160a-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="3160a-105">Ta napaka se lahko manifestira na več načinov, vključno s temi:</span><span class="sxs-lookup"><span data-stu-id="3160a-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="3160a-106">Naprave morda ne bodo sinhronizirane iz ABM/ASM za InTune</span><span class="sxs-lookup"><span data-stu-id="3160a-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="3160a-107">Dodelitev profila članstva morda ne bo uspešna</span><span class="sxs-lookup"><span data-stu-id="3160a-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="3160a-108">Naprave morda ne bodo uspešno dokončale ADE članstva</span><span class="sxs-lookup"><span data-stu-id="3160a-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="3160a-109">Preverite, ali je prišlo do napake pri sinhronizaciji, ki ste jo navedli v konzoli InTune v razdelku **naprave > včlanite naprave > Apple vpis > vpisi žetonov** in preglejte to dokumentacijo, da si ogledate morebitne sanacije:</span><span class="sxs-lookup"><span data-stu-id="3160a-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="3160a-110">Napake za sinhronizacijo v okviru ABM/ASM za avtomatizirane žetone za vpis v sistem iOS/iPadOS in macOS</span><span class="sxs-lookup"><span data-stu-id="3160a-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
