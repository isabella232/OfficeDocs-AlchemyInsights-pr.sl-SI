---
title: Omogočanje uporabe za uporabnika
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971355"
---
# <a name="user-provisioning"></a>Omogočanje uporabe za uporabnika

- Uporabite zmogljivost [omogočanja uporabe na zahtevo,](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) da omogočate uporabo uporabnika in pridobite podrobno diagnostiko o korakih.
- Če želite odpraviti težave, na katere naletite pri omogočanju uporabe za uporabnike in skupine, glejte Vodnik za odpravljanje težav Uporabniki [niso omogočani.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Če opazite, da uporabniki niso omogočani, glejte Omogočanje uporabe [dnevnikov (predogled)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) v Azure Active Directory (AD). Poiščite vnose v dnevniku, ki se nanašajo na določenega uporabnika.
- Občasno znova zaženite omogočanje uporabe, da zasukate vse uporabnike, ki so bili zamujeni v prejšnjem obdobju omogočanja uporabe.
- Uporabnik/skupina morda ni bila omogočana, ker naša storitev še ni imela možnosti, da bi ovrednotila uporabnika. Preglejte navodila, kako dolgo traja omogočanje uporabe ter vrstico napredovanja na strani konfiguracije omogočanja uporabe. Če je stanje stabilen, določeno v razdelku z dodatnimi podrobnostmi, pred datumom, ko je bil uporabnik ustvarjen/posodobljen/izbrisan, to pomeni, da uporabnika še nismo ovrednotili. V tem scenariju je najbolje, da počakate, da se storitev omogočanja uporabe dokonča. Če ste dosegli enako stanje, priporočamo, da v portalu Azure Portal znova zaženete uporabniški vmesnik.
  - Upoštevajte, da je naša storitev seznanjena le s spremembami uporabnika/skupine v izvornem sistemu (Azure Active Directory). Če je uporabnik/skupina odstranjena neposredno v aplikaciji (na primer ServiceNow), teh sprememb ne poznamo in je ne spreminjamo glede na stanje uporabnika v izvornem sistemu. V tem scenariju je najbolje, da spremembo spremenite neposredno v ciljnem programu.
- Naša storitev je ocenila uporabnika/skupino in določila, da ne bi smela biti omogočana:
  - Če ste nastavili obseg na dodeljene uporabnike in skupine, preverite, ali je uporabnik/skupina dodeljena aplikaciji.
  - Če je uporabnik/skupina dodeljena programu, se prepričajte, da ni dodeljena privzeti vlogi za dostop. Te vloge ni mogoče uporabiti za omogočanje uporabe.
  - Če ste nastavili atribut, ki temelji na filtriranju obsega, zagotovite, da uporabnik izpolnjuje navedene pogoje.
  - Če uporabniki že obstajajo v ciljnem sistemu in stanju uporabnika v izvornem in ciljnem ujemanja, ne bomo več akcijo.
- Naša storitev je poskusila na voljo za uporabo uporabnika, zato je bila neuspešna. Za te scenarije preglejte zavihek odpravljanje težav in priporočila v dnevnikih omogočanja uporabe:
  - Morda manjka zahtevan atribut uporabnika v datoteki Azure Active Directory ali pa se ne ujema z obliko zapisa, ki jo zahteva aplikacija tretje osebe. Atribut »Država« za uporabnika je lahko na primer nastavljen na »Združene države« v ZDA.
  - Atribut je referenčni atribut, ki še ne obstaja v ciljnem programu. Referenčni atribut je atribut, ki kaže na drug predmet, na primer uporabnika, ki je član skupine. ID uporabnika bi bil v atributu člana skupine, vendar ga je mogoče obdelati le, če predmet uporabnika, na kateri kaže, že obstaja.
