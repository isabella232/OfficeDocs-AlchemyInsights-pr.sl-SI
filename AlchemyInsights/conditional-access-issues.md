---
title: Težave s pogojnim dostopom
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
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069980"
---
# <a name="conditional-access-issues"></a>Težave s pogojnim dostopom

**Odpravljanje težav z diagnostičnim vpisom**

Hitro lahko ugotovite, kaj se je zgodilo, ali pa diagnosticirate težave, povezane z vpisom uporabnika, tako da uporabite [diagnostično orodje za vpis:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Zaženite diagnostiko vpisa.
1. Poiščite dogodek, ki ga želite analizirati, tako da vnesete podrobnosti o uporabniku, aplikaciji, času vpisa, ID-ju zahteve ali ID-ju korelacije.
1. Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko naredite za spreminjanje (če so potrebne spremembe).

**Navodila za odpravljanje težav z vpisom** 

1. Obiščite stran za vpis v Azure AD.
1. Filtrirajte vpise po uporabniku, časovnem obsegu, aplikaciji, stanju, odjemalski aplikaciji itn.
1. Izberite dogodek vpisa in si oglejte zavihek Pogojni dostop, da si ogledate, kateri pravilniki so bili ovrednoteni.
1. Kliknite vrstico pravilnika, če si želite ogledati podrobnosti pravilnika in razumeti, zakaj se je pravilnik uporabil.

**Orodja za odpravljanje težav s pravilnikom o pogojnem dostopu**

- V načinu samo za poročila lahko ovrednotite pravilnik, ne da bi to vplivalo na uporabnike.
- Z orodjem »kaj-če« lahko simulirate dogodke vpisa in si ogledate, kateri pravilniki veljajo.
- Vpogledi in poročilo o delovnem zvezku prikazuje s seboj učinek posameznega pravilnika v realnem času.

**Pravilniki o zaščiti po osnovnem načrta**

Pravilniki o zaščiti po osnovnem načrta so zastareli. Niso več vsili in bodo kmalu odstranjeni iz portala Azure. Priporočamo, [da omogočite privzete varnostne nastavitve.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Če želite več informacij o pogojnem dostopu, glejte:

[Najboljše prakse pogojnega dostopa v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Pogoji v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolniki v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Mesta v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
