---
title: Napake sinhronizacije samodejnega vpisa v napravo Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448938"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="c5319-102">Napake sinhronizacije samodejnega vpisa v napravo Apple</span><span class="sxs-lookup"><span data-stu-id="c5319-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="c5319-103">» Zaznali smo, da imate enega ali več žetonov ADE/DEP, ki so v stanju napake.</span><span class="sxs-lookup"><span data-stu-id="c5319-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="c5319-104">Dokler stanje napake ni razrešeno za vsak prizadeti žeton, funkcija ADE ne bo delovala po pričakovanjih. ".</span><span class="sxs-lookup"><span data-stu-id="c5319-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="c5319-105">Ta napaka se lahko manifestira na več načinov, vključno s temi:</span><span class="sxs-lookup"><span data-stu-id="c5319-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="c5319-106">Naprave morda ne bodo sinhronizirane iz ABM/ASM za InTune</span><span class="sxs-lookup"><span data-stu-id="c5319-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="c5319-107">Dodelitev profila članstva morda ne bo uspešna</span><span class="sxs-lookup"><span data-stu-id="c5319-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="c5319-108">Naprave morda ne bodo uspešno dokončale ADE članstva</span><span class="sxs-lookup"><span data-stu-id="c5319-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="c5319-109">Preverite, ali je prišlo do napake pri sinhronizaciji, ki ste jo navedli v konzoli InTune v razdelku **naprave > vpis naprav > Apple vpis > vpisi program**.</span><span class="sxs-lookup"><span data-stu-id="c5319-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="c5319-110">Eden najpogostejših vzrokov za napako sinhronizacije je potek trenutnega žetona.</span><span class="sxs-lookup"><span data-stu-id="c5319-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="c5319-111">V številnih primerih bo obnovitev prizadetih žetonov odpravila težavo.</span><span class="sxs-lookup"><span data-stu-id="c5319-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="c5319-112">Če je potekel eden ali več žetonov, si oglejte spodnjo dokumentacijo, ki vam bo v pomoč pri obnovitvi po potrebi:</span><span class="sxs-lookup"><span data-stu-id="c5319-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="c5319-113">Obnovitev avtomatiziranega žetona za vpis v napravo</span><span class="sxs-lookup"><span data-stu-id="c5319-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="c5319-114">Poleg tega si lahko ogledate te dokumente, če si želite ogledati morebitne sanacije za druge napake, ki povzročajo napake pri sinhronizaciji žetona:</span><span class="sxs-lookup"><span data-stu-id="c5319-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="c5319-115">Napake za sinhronizacijo v okviru ABM/ASM za avtomatizirane žetone za vpis v sistem iOS/iPadOS in macOS</span><span class="sxs-lookup"><span data-stu-id="c5319-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="c5319-116">Napake za sinhronizacijo v okviru ABM/ASM za avtomatizirane žetone za vpis v sistem iOS/iPadOS in macOS</span><span class="sxs-lookup"><span data-stu-id="c5319-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
