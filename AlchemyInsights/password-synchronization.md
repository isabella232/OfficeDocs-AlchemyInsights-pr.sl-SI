---
title: Sinhronizacija gesel
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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483084"
---
# <a name="password-synchronization"></a>Sinhronizacija gesel

**Sinhronizacija gesel za gesla sploh ne deluje**

Nekatere pogoste težave, s katerimi se srečujejo uporabniki, ko sinhronizacija z geslom ne deluje:

- Račun imenika Active Directory, ki ga uporablja storitev Azure AD Connect za komunikacijo z imenikom Active Directory na mestu uporabe, ni dodeljen za **ponovitev imenika** in **ponovitev imenika spremeni vsa** dovoljenja, ki jih potrebujete za sinhronizacijo gesel – to morate popraviti tako, da dodelite ta dovoljenja v račun imenika Active Directory.
- Sinhronizacija z geslom za razprševanje je onemogočena, ko je skrbnik **spremenil funkcijo uporabnika** Sign-In iz **sinhronizacije z geslom** na drugo možnost, kot je na primer **zveza z AD FS** v čarovniku za povezovanje v storitvi Azure ad Connect.
- Težave s povezljivostjo z imenikom Active Directory na mestu uporabe. Na primer nekateri krmilniki domen niso dostopni za povezavo s storitvijo Azure AD Connect ali pa so [vrata](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) blokirana s požarnim zidom – to morate popraviti tako, da zagotovite, da je povezljivost med povezovanjem s STREŽNIKOM Azure ad Connect Server in imenikom Active Directory pravilno delovala.
- Strežnik Azure AD Connect Server trenutno poteka v načinu uprizoritev, zaradi česar se strežnik ne more razpršiti z geslom – če želite odpraviti težavo, upoštevajte navodila, opisana v razdelku [Odpravljanje težav z sinhronizacijo gesel s sinhronizacijo storitve AZURE ad Connect – nobena gesla niso sinhronizirana](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Sinhronizacija gesel za gesla ne deluje za nekatere uporabnike**

1. Če ste opazili, da HASH gesla ni sinhroniziran za uporabnika, uporabite opravilo za **Odpravljanje težav** v storitvi Azure ad Connect, da razišče in odpravite težavo. Izvedite ta opravila:

    v. [Zagon opravila za odpravljanje težav v čarovniku](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Uporaba ukaza» cmdlet «za odpravljanje težav pri preverjanju težave pri sinhronizaciji gesel za določeno uporabo](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Uporabniški predmet uporabnika na mestu uporabe je omogočen za **uporabnika mora spremeniti geslo ob naslednji možnosti prijave** . Ko je ta možnost omogočena, je uporabniku dodeljeno začasno geslo in pozvani boste, da spremenite geslo v naslednji prijavi. Azure AD Connect ne sinhronizira začasnih gesel s storitvijo Azure AD.

Če želite odpraviti zgoraj navedeno težavo, izvedite eno od teh opravil:

- Prosite uporabnika, naj se vpiše v program na mestu uporabe (na primer namizje sistema Windows), in spremenite geslo. Novo geslo bo sinhronizirano s storitvijo Azure AD.
- Naj skrbnik posodobi uporabnikovo geslo, ne da bi omogočil, da **mora uporabnik spremeniti geslo ob naslednji prijavi** in dati v skupno rabo novo geslo za uporabnika.

3. Predmet uporabnika imenika Active Directory na mestu uporabe ni **pravilno konfiguriran** za sinhronizacijo predmetov ali sinhronizacijo gesla. Če želite odpraviti to težavo, upoštevajte navodila, opisana v razdelku [Odpravljanje težav z razprševanjem gesel s sinhronizacijo storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







