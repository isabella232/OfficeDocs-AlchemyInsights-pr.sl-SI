---
title: Konfiguracija MIM sinhronizacijske storitve
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482897"
---
# <a name="configure-mim-sync-service"></a>Konfiguracija MIM sinhronizacijske storitve

Microsoft Identity Manager (MIM) storitev sinhronizacije je komponenta MIM. Gre za centralizirano storitev na mestu uporabe, ki shranjuje in združuje informacije za organizacije, ki imajo več imenikov na mestu uporabe in zbirke podatkov. Morda boste lahko odpravili težavo z MIM sinhronizacijo, če je bila težava obravnavana v nedavni posodobitvi na MIM ali je ena od drugih težav, navedenih v spodnjem razdelku.

**Priporočeni koraki**

1. Zagotovite, da uporabljate nedavno posodobitev MIM sinhronizacije in preverite, ali je bila težava odpravljena v posodobitvi, [Če želite ugotoviti](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , ali je prišlo do težave.
2. Če je težava v generičnih protokolih LDAP, generičnih SQL, Lotus Domino ali spletnih storitvah, zagotovite, da uporabljate nedavno posodobitev [generičnih povezovalnikov](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Če se s sporočilom o napaki Ustavi sinhronizacija z napako, se pozanimajte o morebitnih vzrokih v tabeli [kode za zagon](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) .
4. Če se zagon ustavi s **pripono-dll-izjemo** in nato kliknite te besede, da odprete okno **lastnosti predmeta povezovalnika** , in nato kliknite **sledenje sklada...** če si želite ogledati več informacij o osnovnem vzroku, kot je opisano v [priponi-dll-izjema](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Če se v dnevniku dogodkov med sinhronizacijo gesla **prikaže sporočilo 6025 o** komponenti storitve obvestila o spremembi gesla (PCN), preverite navodila za odpravljanje težav s [poročanjem o napakah» PCN «6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Če je popolna sinhronizacija s posrednikom za upravljanje storitve FIM počasna, preverite nastavitev **samodejnega odraščanja** za TempDB, kot je opisano v [odpravljanju težav s počasno ali obešanje polne sinhronizacije](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Če se prikaže sporočilo o napaki ustavljenega strežnika z neuspešnim ustvarjanjem – spletne storitve, ki uporablja posrednika za upravljanje storitve FIM, glejte [Podpora – informacije: neuspešno ustvarjanje – spletne storitve](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) za pregled vzrokov.

