---
title: Odpravljanje napak pri preverjanju pristnosti in avtorizacije za Azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037839"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Odpravljanje napak pri preverjanju pristnosti in avtorizacije za Azure AD (AADSTS)

Če želite odpraviti kode napak za preverjanje pristnosti in avtorizacije (AADSTS), izvedite te priporočene korake:

1. **Kode napak v aplikaciji**

- **Spec OAuth 2.0** https://tools.ietf.org/html/rfc6749#section-5.2 zagotavlja navodila za obravnavanje napak med preverjanjem pristnosti z delom napake pri odgovoru na napako.

    - **napaka**: niz kode napake, s katerim lahko razvrstite vrste napak, ki se pojavijo, in jih uporabite, če želite reagirati na napake.
    - Polje» **napaka** «ima več možnih vrednosti – preglejte povezave do dokumentacije protokola in specifikacije OAuth 2,0, če želite več informacij o določenih napakah in kako reagirati nanje.

- Tukaj je primer odziva na vzorčno napako:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Informacije o kodi za iskanje trenutne kode**

- Kode napak in sporočila se lahko spremenijo. Če želite najnovejše informacije, si oglejte https://login.microsoftonline.com/error stran, če želite poiskati opise napak AADSTS, popravke in nekatere predlagane rešitve.
- Prav tako lahko poiščete in odpravljate težave z [AADSTS kodami napak](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , ki so navedene v članku [kode napake za preverjanje pristnosti in avtorizacije](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Poiščite pomoč**

- [Možnosti podpore in pomoči za razvijalce](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – Če potrebujete odgovor na vprašanje ali pomoč pri reševanju težave, ki ni zajeta v naši dokumentaciji, je morda čas, da poiščete strokovnjake za pomoč. V tem članku je na voljo več predlogov za pridobivanje odgovorov na vaša vprašanja, ko razvijate programe, ki se povezujejo z Microsoftovo platformo Identity.








