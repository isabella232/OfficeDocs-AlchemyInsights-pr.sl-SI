---
title: 646 Kako konfigurirati AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963659"
---
# <a name="configure-sync-features"></a>Konfiguracija funkcij sinhronizacije

Azure AD Povezovalnik vključuje več funkcij, ki so privzeto omogočene ali jih lahko omogočite pozneje. Nekatere funkcije zahtevajo dodatno konfiguracijo v določenih okoljih.

- [Omejitve filtriranja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) so predmeti sinhronizirani z imenikom Azure AD. Privzeto so sinhronizirani vsi uporabniki, stiki, skupine in Windows 10 računi računalnika. Vključite ali izključite lahko predmete na podlagi domen, OU-ov ali drugih atributov.

- [Sinhronizacija z gesli](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizira gesli iz imenika Active Directory na mestu uporabe z imenikom Azure AD. To omogoča upravljanje gesel na enem mestu, vendar z istim geslom v okoljih na mestu uporabe in v oblaku. Ker je imenik Active Directory avtoritativen vir, lahko uporabljate svoje pravilnike za gesla.

- [Samopostrežna ponastavitev gesla omogoča](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) uporabnikom, da ponastavijo svoja gesla v oblaku, medtem ko še vedno uporabljajo pravilnik za gesla na mestu uporabe.

- [Funkcija povratnega pisanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) naprave omogoča, da se registrirane naprave v imeniku Azure AD zapišejo nazaj v imenik Active Directory na mestu uporabe, tako da jih je mogoče uporabiti za pogojni dostop.

- [Preprečevanje nenamernih brisanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočeno, da preprečite preveč hkratnega brisanja predmetov (več kot 500 predmetov na sinhronizacijo). To nastavitev lahko spremenite tako, da ustreza potrebam vaše organizacije.

- [Samodejna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) nadgradnja je privzeto omogočena za hitre namestitve in zagotavlja, da je vaša različica programa Azure AD Povezovalnik vedno posodobljena.
