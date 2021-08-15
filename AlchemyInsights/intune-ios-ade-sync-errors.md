---
title: Napake pri sinhronizaciji samodejnega včlanitve naprave Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013764"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Napake pri sinhronizaciji samodejnega včlanitve naprave Apple

»Zaznali smo, da imate enega ali več žetonov ADE/DEP, ki so v stanju napake. Dokler stanje napake ne bo odpravljeno za vsak prizadet žeton, funkcija ADE ne bo delovala v skladu s pričakovanji.«.

Ta napaka se lahko pojavi na več načinov, med drugim tudi na te načine:

1. Naprave se morda ne bodo sinhronizirale iz ABM/ASM z Intune
2. Dodelitev profila za včlanitev morda ne bo na
3. Naprave morda ne bodo uspešno dokončale včlanitve ADE

Preverite napake pri sinhronizaciji, ki so se prijavile v konzoli Zatune v razdelku Naprave > včlanitve naprave > včlanitev družbe **Apple > včlanitev** v program.

Eden od najpogostejših vzrokov za napako pri sinhronizaciji je potek trenutnega žetona. V številnih primerih lahko to težavo odpravite s podaljšanjem prizadetega žetona.

Če je eden ali več žetonov poteklo, si oglejte to dokumentacijo za pomoč pri obnovitvi žetonov, kot je primerno:

[Podaljšanje žetona za avtomatizirano včlanitev naprave](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Poleg tega si lahko ogledate to dokumentacijo, da si ogledate morebitne popravkov za druge napake, zaradi katerih je prišlo do napak pri sinhronizaciji žetonov:

[Napake pri sinhronizaciji ABM/ASM za žetone za sistem iOS/iPadOS in macOS Automated Device Enrollment](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Napake pri sinhronizaciji ABM/ASM za žetone za sistem iOS/iPadOS in macOS Automated Device Enrollment](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
