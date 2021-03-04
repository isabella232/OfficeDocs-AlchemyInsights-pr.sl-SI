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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Napake sinhronizacije samodejnega vpisa v napravo Apple

» Zaznali smo, da imate enega ali več žetonov ADE/DEP, ki so v stanju napake. Dokler stanje napake ni razrešeno za vsak prizadeti žeton, funkcija ADE ne bo delovala po pričakovanjih. ".

Ta napaka se lahko manifestira na več načinov, vključno s temi:

1. Naprave morda ne bodo sinhronizirane iz ABM/ASM za InTune
2. Dodelitev profila članstva morda ne bo uspešna
3. Naprave morda ne bodo uspešno dokončale ADE članstva

Preverite, ali je prišlo do napake pri sinhronizaciji, ki ste jo navedli v konzoli InTune v razdelku **naprave > vpis naprav > Apple vpis > vpisi program**.

Eden najpogostejših vzrokov za napako sinhronizacije je potek trenutnega žetona. V številnih primerih bo obnovitev prizadetih žetonov odpravila težavo.

Če je potekel eden ali več žetonov, si oglejte spodnjo dokumentacijo, ki vam bo v pomoč pri obnovitvi po potrebi:

[Obnovitev avtomatiziranega žetona za vpis v napravo](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Poleg tega si lahko ogledate te dokumente, če si želite ogledati morebitne sanacije za druge napake, ki povzročajo napake pri sinhronizaciji žetona:

[Napake za sinhronizacijo v okviru ABM/ASM za avtomatizirane žetone za vpis v sistem iOS/iPadOS in macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Napake za sinhronizacijo v okviru ABM/ASM za avtomatizirane žetone za vpis v sistem iOS/iPadOS in macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
