---
title: Težave pri razvoju programov z API-ji
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975018"
---
# <a name="issues-developing-applications-with-apis"></a>Težave pri razvoju programov z API-ji

Za začetek uporabe API-ja v storitvi Azure Active Directory je na [sporedu vodnik AZURE ad GRAPH API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , ali pa si oglejte dokumentacijo priročnika [interaktivnih](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)grafičnih grafikonov Azure ad.

**Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (graf ZVOČNIh grafikonov)**

Z **začetkom junija 30th 2020** ne bomo več dodali nobenih novih funkcij v knjižnice adal in Azure ad Graph. Še naprej bomo zagotavljali tehnično podporo in varnostne posodobitve, vendar ne boste mogli več posredovati posodobitev funkcij.

Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.

Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo prejeli nobene tehnične podpore ali varnostnih posodobitev.

Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.

**Selitev v knjižnice ADAL**

Priporočamo, da posodobite [Microsoftovo knjižnico za preverjanje pristnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki ima najnovejše funkcije in varnostne posodobitve.

Če uporabljate Microsoft apps, veste, da je Microsoft v postopku selitve svojih programov v MSAL z rokom za konec podpore, s čimer zagotovite, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.

1. [Preberite pogosta vprašanja o knjižnice adal](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Preberite več o tem, kako preseliti aplikacije na osnovi na platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, vam priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne ISVs ali ponudnike programov. Microsoftova podpora vam omogoča tudi seznam vseh programov, ki niso Microsoftovi za knjižnice ADAL, v najemniku.

**Selitev diagrama ZVOČNIh grafikonov**

Za programe, ki uporabljajo grafiko Azure AD Graph, upoštevajte navodila za selitev [programov AZURE ad Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Naš kontrolni seznam selitve zagotavlja uvodno mesto](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. V portalu za registracijo aplikacije Azure so prikazani programi, ki uporabljajo ZVOČNI diagram. Priporočamo vam, da pregledate vse izvorne kode programov in po potrebi poiščete vse ponudnike ISVs ali aplikacije. Microsoftova podpora vam omogoča tudi seznam vseh uporab ZVOČNIh grafikonov v najemniku.
1. Če želite za program dostopati do podatkov v programu Microsoft Graph, ga mora uporabnik ali skrbnik dodeliti pravilnim dovoljenjem prek postopka soglasja. [Sklici na dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) navajajo dovoljenja, povezana z vsakim glavnim naborom API-jev Microsoft Graph. Na voljo so tudi navodila za uporabo dovoljenj.
