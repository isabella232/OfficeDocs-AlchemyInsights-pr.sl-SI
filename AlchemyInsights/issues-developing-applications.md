---
title: Težave pri razvoju aplikacij
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013440"
---
# <a name="issues-developing-applications"></a>Težave pri razvoju aplikacij

Če želite odpraviti najpogostejše težave pri Azure Active Directory aplikacij (AD), glejte te članke:

- [Vidim težave z vpisom v aplikacije le z brskalnikom Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ne vem, kako spremenim privzete življenjske dobe žetona za svojo aplikacijo](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Ne vem, kako deluje soglasje za aplikacijo](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ne vem, kako dodelim dovoljenja za aplikacijo](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ne razumem razlike med pooblaščenimi dovoljenji in dovoljenji za aplikacijo](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Konec podpore za knjižnico za preverjanje Azure Active Directory pristnosti (ADAL) in Azure AD Graph API (AAD Graph)***

- Od 30. junija 2020 ne dodajamo več novih funkcij v knjižnico Azure Active Directory Authentication Library (ADAL) in vmesnik API za Azure AD Graph (AAD Graph). Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.

- 30. junija 2022 se je končala podpora za ADAL in AAD Graph, prav tako ni več na voljo tehnična podpora in varnostne posodobitve. Posledično so posledice za to stanje:

    - Aplikacije, ki uporabljajo ADAL v obstoječih različicah operacijskega sistema, bodo po tem obdobju še naprej delovale, vendar zanje ne bo več mogoče pridobiti tehnične podpore ali varnostnih posodobitev.

    - Aplikacije, ki uporabljajo AAD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne Graph AAD

**Selitev ADAL**

Če uporabljate Microsoftove aplikacije, priporočamo nadgradnjo na Microsoftovo knjižnico preverjanja pristnosti (MSAL), ki ima najnovejše funkcije in varnostne posodobitve. To priporočilo je v kontekstu, ko Microsoft odlaša postopek selitve aplikacij v MSAL do roka za končanje podpore. 

Microsoft lahko selitev njegovih aplikacij v storitev MSAL zagotovi, da imajo aplikacije prednosti zaradi trenutnih izboljšav varnosti in funkcij storitve MSAL.

1. [Preberite pogosta vprašanja o knjižnici ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Več informacij o selitvi aplikacij glede na platformo](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Če potrebujete pomoč pri razumevanju, katero od aplikacij uporabljate ADAL, priporočamo, da pregledate izvorno kodo aplikacije in, če je na voljo, se obrnite na neodvisne ponudnike programske opreme (ISVs) ali ponudnike aplikacij. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za aplikacije, ki uporabljajo AAD Graph, upoštevajte naša navodila za selitev aplikacije AAD Graph v Microsoft Graph:

1. [Kontrolni seznam za selitev vključuje točko za začetek izvajanja postopka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate vso izvorno kodo aplikacije in, če je na voljo, se obrnite na neodvisne ponudnike programske opreme (ISVs) ali ponudnike aplikacij. Microsoftova podpora vam lahko zagotovi tudi informacije o uporabi storitve AAD Graph v vašem najemniku.







