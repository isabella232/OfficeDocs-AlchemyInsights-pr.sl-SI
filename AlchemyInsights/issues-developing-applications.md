---
title: Težave z razvojem programov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974767"
---
# <a name="issues-developing-applications"></a>Težave z razvojem programov

Če želite odpraviti najpogostejše težave pri gradnji programov Azure Active Directory (AD), si oglejte te članke:

- [Vidim težave pri vpisu v program le z brskalnikom Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ne vem, kako naj spremenim privzete nastavitve žetona za moj program](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Sem zbegan o tem, kako deluje soglasje aplikacije](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ne vem, kako dodeliti dovoljenja za moj program](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ne razumem razlike med delegiranimi in dovoljenji za uporabo](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice adal) in AZURE ad GRAPH API (zvočni grafikon)** _

- Z začetkom junija 30th 2020 ne bomo več dodali nobenih novih funkcij v knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (ZVOČNI grafikon). Še naprej bomo zagotavljali tehnično podporo in varnostne posodobitve, vendar ne boste mogli več posredovati posodobitev funkcij.

- Z začetkom junija 30th 2022 bomo zaključili podporo za knjižnice ADAL in ZVOČNI diagram ter ne bodo več zagotavljali tehnične podpore ali varnostnih posodobitev. Zaradi tega pogoja so te posledice:

    - Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo prejeli nobene tehnične podpore ali varnostnih posodobitev.

    - Programi, ki uporabljajo ZVOČNI diagram, po tem času morda ne bodo več prejemali odgovorov iz končne točke v grafu ZVOČNIka

_ *Knjižnice adal selitev**

Če uporabljate Microsoft apps, priporočamo, da posodobite Microsoftovo knjižnico za preverjanje pristnosti (MSAL), ki ima najnovejše funkcije in varnostne posodobitve. To priporočilo je v kontekstu Microsoft, ki uvaja postopek selitve svojih programov v MSAL z rokom konca podpore. 

Selitev Microsoft svojih aplikacij v MSAL zagotavlja, da bodo aplikacije izkoristile prednosti sprotne varnosti in izboljšav funkcij MSAL.

1. [Preberite pogosta vprašanja o knjižnice ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Preberite več o tem, kako preseliti aplikacije na osnovi na platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne neodvisne prodajalce programske opreme (ISVs) ali ponudnike programov. Microsoftova podpora vam omogoča tudi seznam vseh programov, ki niso Microsoftovi za knjižnice ADAL, v najemniku.

**Selitev diagrama ZVOČNIh grafikonov**

Za programe, ki uporabljajo ZVOČNI graf, upoštevajte naše napotke za selitev programov ZVOČNIh grafikonov v Microsoft Graph:

1. [Naš kontrolni seznam selitve zagotavlja uvodno mesto](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. V portalu za registracijo aplikacije Azure so prikazani programi, ki uporabljajo ZVOČNI diagram. Priporočamo vam, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne neodvisne prodajalce programske opreme (ISVs) ali ponudnike programov. Microsoftova podpora vam omogoča tudi informacije o uporabi ZVOČNIh grafikonov v najemniku.







