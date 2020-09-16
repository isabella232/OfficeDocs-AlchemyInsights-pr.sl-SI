---
title: 902 (napake sinhronizacije zaradi podvojenih predmetov)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737357"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Napake sinhronizacije zaradi podvojenih predmetov

Ko se sinhronizacija imenika konča v programu Microsoft 365, se lahko prikaže eno od teh sporočil o napaki:

- Tega predmeta ni mogoče posodobiti v storitvi Microsoft Online Services, ker so v teh atributih, povezanih s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v lokalnem imeniku.

- Sinhroniziran predmet z istim naslovom strežnika proxy že obstaja v vašem imeniku storitve Microsoft Online Services.

- Tega predmeta ni mogoče posodobiti, ker so v teh atributih, povezanih s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v lokalnih imeniških storitvah: UserPrincipalName.

Če želite prepoznati in odpraviti težavo, prenesite in zaženite [orodje za sanacijo napak v IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Če želite več informacij, glejte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
