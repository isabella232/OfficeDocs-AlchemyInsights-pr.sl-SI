---
title: 646 kako konfigurirate AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704505"
---
# <a name="configure-sync-features"></a>Konfiguracija funkcij sinhronizacije

V storitvi Azure AD Connect so na voljo številne funkcije, ki so privzeto omogočene ali pa jih lahko omogočite pozneje. Nekatere funkcije zahtevajo dodatno konfiguracijo v določenih okoljih.

- Omejitve [filtriranja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) predmeti se sinhronizirajo s storitvijo Azure ad. Privzeto so vsi uporabniki, stiki, skupine in računi v računalniku s sistemom Windows 10 sinhronizirani. Predmete lahko vključite ali izključite na osnovi domen, organizacijskih ali drugih atributov.

- [Sinhronizacija gesla za razprševanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizira geslo razpršitve iz imenika Active Directory na mestu uporabe v storitvi Azure ad. S tem lahko upravljate upravljanje gesel na enem mestu, vendar uporabite enako geslo v okoljih na mestu uporabe in v oblaku. Ker je Active Directory avtoritativni vir, lahko uporabite svoje pravilnike za gesla.

- [Samopostrežno ponastavitev gesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) uporabnikom omogoča, da ponastavijo svoja gesla v oblaku, medtem ko še vedno uporabljajo pravilnike za gesla na mestu uporabe.

- [Naprava nepotrjenim](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogoča, da se registrirane naprave v storitvi Azure ad zapišejo v imenik Active Directory na mestu uporabe, da jih je mogoče uporabiti za pogojni dostop.

- [Preprečevanje nenamernih brisanj](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočeno, da preprečite preveč hkratnih brisanj predmetov (več kot 500 predmetov na sinhronizacijo). To nastavitev lahko spremenite, da zadovoljite potrebe organizacije.

- [Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je privzeto omogočena za ekspresne naprave in zagotavlja, da je različica storitve Azure ad Connect vedno aktualna.
