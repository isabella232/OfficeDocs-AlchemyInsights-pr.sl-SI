---
title: Sinhronizacija gesla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960851"
---
# <a name="password-synchronization"></a>Sinhronizacija gesla

**Sinhronizacija z gesli sploh ne deluje**

Nekatere pogoste težave, do katerih pride, ko sinhronizacija hash gesla ne deluje:

- Računu imenika Active Directory, ki ga uporablja Azure AD Povezovalnik za  komunikacijo z  imenikom Active Directory na mestu uporabe, ni dodeljena replikacijam sprememb imenika in spremembam v imeniku . Vsa dovoljenja, ki so zahtevana za sinhronizacijo gesel – to morate popraviti tako, da podelite ta dovoljenja računu imenika Active Directory.
- Sinhronizacija hash gesla je onemogočena, ko skrbnik  v čarovniku za azure AD Povezovalnik način uporabniškega Sign-In iz sinhronizacije gesel spremeni v  drugo možnost, na primer Povezovanje z ad **FS** – to težavo lahko odpravite tako, da znova omogočite funkcijo sinhronizacije z geslom v čarovniku za Azure AD Povezovalnik.
- Težava s povezljivostjo z imenikom Active Directory na mestu uporabe. Nekateri krmilniki domen na primer niso dostopni s storitvijo [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Povezovalnik ali pa so zahtevana vrata blokirala požarni zid – to morate popraviti tako, da zagotovite pravilno delovanje povezljivosti med strežnikom Azure AD Povezovalnik in imenikom Active Directory na mestu uporabe.
- Strežnik Azure AD Povezovalnik je trenutno v načinu uprizoritev, zaradi česar strežnik ne bo mogel do razčlenjevati gesel – če želite odpraviti težavo, upoštevajte navodila, opisana v razdelku Odpravljanje težav s sinhronizacijo gesel s sinhronizacijo imenika Azure AD Povezovalnik – gesla niso [sinhronizirana.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Sinhronizacija z gesli ne deluje za nekatere moje uporabnike**

1. Če ste opazili, da se hash gesla ne  sinhronizira za uporabnika, uporabite opravilo za odpravljanje težav v imeniku Azure AD Povezovalnik raziščite in odpravite težavo. Izvedite ta opravila:

    a. [Zagon opravila za odpravljanje težav v čarovniku](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Uporabite ukaz »cmdlet« za odpravljanje težav, da raziščete težavo s sinhronizacijo hash gesla za določeno uporabo.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Uporabniški predmet Active Directory na mestu uporabe je omogočen za Uporabnika mora spremeniti **geslo ob naslednji možnosti** prijave. Ko je ta možnost omogočena, je uporabniku dodeljeno začasno geslo in ob naslednji prijavi pozvan k spremembi gesla. Azure AD Povezovalnik ne sinhronizira začasnih gesel z imenikom Azure AD.

Če želite odpraviti zgornjo težavo, izvedite enega od teh opravil:

- Prosite uporabnika, da se vpiše v aplikacijo na mestu uporabe (na primer Windows Desktop) in spremeni geslo. Novo geslo bo sinhronizirano z imenikom Azure AD.
- Naj skrbnik posodobi geslo uporabnika, ne da bi omogočil možnost Uporabnik mora spremeniti geslo ob naslednji prijavi **in** nato novo geslo deliti z uporabnikom.

3. Uporabniški predmet imenika Active Directory na mestu uporabe ni **pravilno konfiguriran za sinhronizacijo** predmetov ali sinhronizacijo gesel. Če želite odpraviti to težavo, upoštevajte navodila, opisana v poglavju Odpravljanje težav s sinhronizacijo gesla [z orodjem Azure AD Povezovalnik sinhronizacijo.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







