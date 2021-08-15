---
title: Težave pri razvoju aplikacij z API-ji
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013476"
---
# <a name="issues-developing-applications-with-apis"></a>Težave pri razvoju aplikacij z API-ji

Če želite začeti uporabljati Azure Active Directory Graph API, glejte Vodnik za hiter začetek Graph API za Azure AD Graph ali pa si oglejte [interaktivno](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)dokumentacijo z Graph za API za Azure [AD.](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro)

**Konec podpore za knjižnico za preverjanje Azure Active Directory pristnosti (ADAL) in Azure AD Graph API (AAD Graph)**

**Od 30. junija 2020** ne bomo več dodajali novih funkcij v ADAL in Azure AD Graph. Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.

**Od 30. junija 2022** se bo končala podpora za ADAL in Azure AD Graph in ne bomo več zagotavljali tehnične podpore ali varnostnih posodobitev.

Aplikacije, ki uporabljajo ADAL v obstoječih različicah operacijskega sistema, bodo po tem obdobju še naprej delovale, vendar zanje ne bo več mogoče pridobiti tehnične podpore ali varnostnih posodobitev.

Aplikacije, ki uporabljajo Azure AD Graph po tem času morda ne bodo več prejemali odgovorov iz končne točke Graph Azure AD.

**Selitev ADAL**

Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve.

Če uporabljate Microsoftove aplikacije, veste, da Microsoft do konca roka za podporo izvaja selitev svojih aplikacij v MSAL, pri čemer jim zagotavlja, da bo izkoristil prednosti trenutnih izboljšav MSAL in funkcij.

1. [Preberite pogosta vprašanja o storitvi ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Preberite več o selitvi aplikacij na osnovi platforme.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Če potrebujete pomoč pri razumevanju, katero od aplikacij uporabljate ADAL, vam priporočamo, da pregledate izvorno kodo vseh aplikacij in se, če je na voljo, preglejte morebitne ponudnike internetnih storitev ali ponudnike aplikacij. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za aplikacije, ki uporabljajo Azure AD Graph, upoštevajte naša navodila za selitev [aplikacij Azure AD Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Kontrolni seznam za selitev vključuje točko za začetek izvajanja postopka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam lahko zagotovi tudi seznam vseh AAD-Graph uporabe v vašem najemniku.
1. Če želite, da vaša aplikacija dostopa do podatkov v Graph Microsoft Graph, ji mora uporabnik ali skrbnik prek postopka podelitve soglasja podeliti ustrezna dovoljenja. V [sklicu Graph Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) navedeni dovoljenji, ki so povezana z vsakim glavnim naborom API-jev Graph Microsoft Graph. V njem so na voljo tudi navodila za uporabo dovoljenj.
