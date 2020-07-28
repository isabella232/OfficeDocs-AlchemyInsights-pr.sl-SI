---
title: Apple MDM Push Certificate ni bil nastavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440010"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Certificate ni bil nastavljen

Apple MDM Push Certificate (znan tudi kot apple push notification service (APNS) ni bil konfiguriran za vašo naročnino. Brez apple MDM Push certificate nastavljen, ne morete vpisati in upravljati iOS in Mac OS naprave. Ko dodate potrdilo v intune, lahko uporabniki namestijo aplikacijo Portal podjetja, da včlanejo svoje naprave s sistemom iOS.

1. Izberite **"Strinjam se."** dati Microsoftu dovoljenje za pošiljanje podatkov apple.

2. Izberite **Prenesite zahtevo za** podpisovanje potrdila za intune, ki je potrebna za ustvarjanje potisnega potrdila Apple MDM. Datoteka se uporablja za zahtevo certifikata odnosa zaupanja iz portala apple push certifikatov.

3. Izberite **Ustvari push potrdilo MDM, da** se poišate na portal apple push certifikatov. Vpišite se s svojim podjetjem Apple ID in nato **izberite Ustvari potrdilo**. Izberite **Izberi datoteko**, poiščite datoteko zahteve za podpisovanje certifikatov in nato **izberite Prenesi**. Na strani Potrditev izberite **Prenesi,** da prenesete datoteko s potrdilom (.pem) in jo shranite lokalno.
 
**Opomba:** Potrdilo je povezano z APPLE ID-jem, ki se uporablja za njegovo ustvarjanje. Za opravila upravljanja uporabite podjetje Apple ID in preverite, ali nabiralnik nadzoruje več oseb ali uporabljate seznam prejemnikov. Nikoli ne uporabljajte osebnega Apple ID-ja. Uporabite isti Apple ID obnoviti Apple Push certificate vsakih 12 mesecev.
 
4. Vnesite Apple ID, ki se uporablja za ustvarjanje push certifikata Apple MDM. Ta ID zasnemite kot opomnik za čas, ko morate obnoviti potrdilo.

5. Odprite datoteko s potrdilom (.pem), izberite **Odpri**in nato **Prenesi**. S potisnim potrdilom lahko Intune vpiše in upravlja naprave Apple.