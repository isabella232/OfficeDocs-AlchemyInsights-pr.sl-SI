---
title: 902 (Napake pri sinhronizaciji zaradi podvojenih predmetov)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998810"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Napake pri sinhronizaciji zaradi podvojenih predmetov

Ko se sinhronizacija imenika konča v storitvi, se lahko prikaže eno od teh Microsoft 365:

- Tega predmeta ni mogoče posodobiti v storitvah Microsoft Online Services, ker imajo ti atributi, povezani s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v vašem lokalnem imeniku.

- Sinhronizirani predmet z istim naslovom proxy že obstaja v imeniku storitev Microsoft Online Services.

- Tega predmeta ni mogoče posodobiti, ker imajo ti atributi, povezani s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v vaših lokalnih imeniških storitvah: UserPrincipalName.

Če želite odpraviti težavo, prenesite in zaženite orodje za [odpravljanje napak IdFix DirSync.](https://github.com/Microsoft/idfix)

Če želite več informacij, [glejte KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
