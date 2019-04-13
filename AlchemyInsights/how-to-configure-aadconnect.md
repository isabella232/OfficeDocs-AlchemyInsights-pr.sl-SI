---
title: 646 kako nastaviti AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856672"
---
# <a name="configure-sync-features"></a>Nastavitev sinhronizacije funkcij

Sinje AD Connect vključuje številne funkcije, ki so privzeto omogočen, ali ki lahko kasneje. Nekatere funkcije zahtevajo dodatno konfiguracijo v posebnih okoljih.

- [Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) omejitev predmetov sinhronizirajo Azure AD. Privzeto, vsi uporabniki, stike, skupine, in Windows 10 računov računalnika sinhronizirajo. Lahko vključujejo ali izključujejo predmete, ki temeljijo na domene, OU-ji, ali druge lastnosti.

- [Parola haše sinhronizacija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizira geslo haše iz krajevnega imenika Active Directory za modro AD. To omogoča upravljanje gesel na enem mestu, ampak uporabite isto geslo krajevnimi in oblak okoljih. Ker aktivni imenik je avtoritativni vir, lahko uporabite svoje pravilnike za gesla.

- [Samopostrežno parola prikrivati (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogučiti uporabnik v prikrivati svoja gesla v oblaku, medtem ko še vedno uporabi pravilnik za gesla krajevne.

- [Writeback naprava](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogoča registrirani naprav v sinje oglas za pisanje nazaj na imeniku Active Directory, se lahko uporabijo za pogojni dostop.

- [Preprečevanje nenamernega izbriše](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočen za pomoč pri preprečevanju preveč sočasno predmet Izbrisi (več kot 500 predmetov na sinhronizacijo). Spremenite lahko te nastavitve za potrebe vaše organizacije.

- [Samodejno nadgradnjo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je privzeto omogočen za hitre naprave in pomaga zagotoviti vašo različico Azure AD povezavo je vedno Trenutna.
