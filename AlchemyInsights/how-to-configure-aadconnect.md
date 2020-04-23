---
title: 646 kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722579"
---
# <a name="configure-sync-features"></a>Konfiguracija funkcij sinhronizacije

Azure AD Connect vključuje več funkcij, ki so privzeto omogočene, ali pa jih lahko pozneje omogočite. Nekatere funkcije zahtevajo dodatno konfiguracijo v določenih okoljih.

- [Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) omejuje, da so predmeti sinhronizirani s storitvijo Azure ad. Privzeto se sinhronizirajo vsi uporabniki, stiki, skupine in računi računalnika s sistemom Windows 10. Predmete lahko vključite ali izključite na podlagi domen, OUs ali drugih atributov.

- [Sinhronizacija za razprševanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) gesel sinhronizira razprševanje gesla iz krajevnega imenika Active Directory v Azure ad. To omogoča upravljanje gesel na enem mestu, vendar Uporaba istega gesla v krajevnih in oblačnih okoljih. Ker je Active Directory avtoritativni vir, lahko uporabite svoje pravilnike o geslih.

- [Samopostrežna ponastavitev gesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogoča uporabnikom, da ponastavijo svoja gesla v oblaku, medtem ko še vedno uporabljajo krajevni pravilnik o geslih.

- [Naprava writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogoča, da se registrirane naprave v storitvi Azure ad zapišemo nazaj v krajevni imenik Active Directory, tako da jih je mogoče uporabiti za pogojni dostop.

- [Preprečite nenamerno brisanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočeno, da se prepreči preveč hkratnih brisanja predmetov (več kot 500 predmetov na sinhronizacijo). To nastavitev lahko spremenite tako, da ustreza potrebam vaše organizacije.

- [Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je privzeto omogočena za hitre namestitve in pomaga zagotoviti, da je vaša različica Azure ad Connect vedno aktuna.
