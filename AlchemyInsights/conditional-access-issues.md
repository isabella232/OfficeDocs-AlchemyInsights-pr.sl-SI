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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015002"
---
# <a name="conditional-access-issues"></a>Težave s pogojnim dostopom

**Odpravljanje težav z diagnostičnim vpisom**

Hitro lahko ugotovite, kaj se je zgodilo ali diagnosticirali težave, povezane z uporabniškim vpisom, in sicer tako, da uporabite [diagnostično prijavo](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Zaženite diagnostiko za vpis.
1. Poiščite dogodek, ki ga želite analizirati, in sicer tako, da vnesete podrobnosti o uporabniku, aplikaciji, času vpisa, ID-ju zahteve ali korelaciji.
1. Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko izvedete, če želite spremeniti (če so potrebne spremembe).

**Navodila za odpravljanje težav z vpisom** 

1. Pomaknite se na stran za vpis v Azure AD.
1. Vpisi filtra po uporabnikih, časovnem obsegu, aplikaciji, stanju, odjemalskem programu in tako dalje.
1. Izberite dogodek za vpis in si oglejte zavihek pogojni dostop, da si ogledate, katere pravilnike ste ocenili.
1. Kliknite vrstico pravilnika, če si želite ogledati podrobnosti pravilnika in razumeti, zakaj je uporabljen.

**Orodja za odpravljanje težav s pogojnim dostopom**

- Način» samo za poročilo «vam omogoča, da ocenite pravilnik brez vpliva uporabnikov.
- Orodje» kaj-če «vam omogoča simulacijo dogodkov za vpis in ogled pravilnikov.
- Delovni zvezek za vpoglede in poročanje prikaže sprotni vpliv posameznih pravilnikov.

**Pravilniki o zaščiti osnovnih podatkov**

Pravilniki o zaščiti po osnovnem načrtu so bili zastareli. Niso več uveljavljene in bodo kmalu odstranjene iz portala Azure. Priporočamo, da omogočite [varnostne privzete nastavitve](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Če želite več informacij o pogojnem dostopu, glejte:

[Najboljši načini za pogojni dostop v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Pogoji v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolniki v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokacije v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
