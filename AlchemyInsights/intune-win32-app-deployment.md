---
title: InTune za uvajanje aplikacije Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461993"
---
# <a name="intune-win32-app-deployment"></a>InTune za uvajanje aplikacije Win32

Microsoft InTune omogoča Win32 aplikacije, vključno z, vendar ne omejeno na MSI in. EXE je treba uvesti v naprave s sistemom Windows 10. Uporabljeni mehanizem za uvajanje zahteva, da je v ciljni napravi prisoten ukaz» InTune «(IME). IME bo samodejno nameščeno zaradi usmerjanja skripta PowerShell ali uvedbe aplikacije Win32 v uporabnika/napravo.

Na voljo je tudi nabor predpogojev, ki jih je treba izpolniti, da se uvede Win32 aplikacije, ki vključujejo:

- Podprte platforme: Windows 10 različica 1607 ali novejša (različica Enterprise, Pro in Education).
- Podprta arhitektura: x86 in x64.
- Upravljanje naprav:» ZVOČNa skupina «in» samodejno vpisan «(vključno s povezanimi hibridnimi domenami in samodejnim vpisom pravilnika skupine).
- Oblika paketa aplikacije:. **intunewin**  datoteka, ki jo je pripravila [Orodja Microsoft Win32 Content prep](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Omejitve
    - Največja velikost: 8GB.
    - Nepodprta arhitektura: orožje.

Če želite informacije, povezane s temi koraki, preglejte dokument»[Dodaj, dodeli in spremljajte aplikacijo Win32 «v programu Microsoft InTune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add).

Podrobnosti o odpravljanju težav z uvajanjem programov v sistemu Windows, vključno z aplikacijami Win32, si lahko ogledate v teh dokumentih

- [Odpravljanje težav z namestitvijo aplikacije](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Odpravljanje težav z Win32 programi](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)