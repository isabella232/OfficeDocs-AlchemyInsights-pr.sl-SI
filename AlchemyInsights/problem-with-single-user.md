---
title: Težava z enim uporabnikom
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
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960167"
---
# <a name="problem-with-single-user"></a>Težava z enim uporabnikom

- Uporabnik morda še ni bil omogočan, ker storitev še ni imela možnosti, da bi ovrednotila uporabnika. Preglejte navodila, kako dolgo traja omogočanje uporabe ter vrstico napredovanja na strani konfiguracije omogočanja uporabe. Če je stanje stabilen, določeno v razdelku z dodatnimi podrobnostmi, pred datumom, ko je bil uporabnik ustvarjen/posodobljen/izbrisan, to pomeni, da uporabnika še nismo ovrednotili. V tem scenariju je najbolje, da počakate, da se storitev omogočanja uporabe dokonča.

  - Upoštevajte, da je naša storitev seznanjena le s spremembami uporabnika v izvornem sistemu (CLOUD HR). V izvornem sistemu imenika Azure AD mora biti veljavna sprememba, da zazna spremembo in jo preli v imenik Active Directory.
- Storitev omogočanja uporabe je ovrednotila uporabnika in določila, da ne bi smela biti omogočanja uporabe:
  - Če ste nastavili atribut, ki temelji na filtriranju obsega, zagotovite, da uporabnik izpolnjuje navedene pogoje.
  - Če uporabniki že obstajajo v ciljnem sistemu in stanju uporabnika v izvornem in ciljnem ujemanja, ne bomo več akcijo.
- Storitev omogočanja uporabe je poskusila omogočati uporabo uporabnika, zato ni uspela. Za te scenarije preglejte zavihek odpravljanje težav in priporočila v dnevnikih omogočanja uporabe:
  - Morda manjka zahtevani atribut uporabnika v imeniku Active Directory na mestu uporabe ali imeniku Azure AD. Na primer, pravila generacije userPrincipalName ali sAMAccountName ne ustvarjajo pravih vrednosti.
  - Ujemajoči se atribut (običajno employeeId) ni razrešen za enoličnega uporabnika v imeniku Active Directory na mestu uporabe ali imeniku Azure AD. Obstajata na primer dva uporabnika z istim iD-jem zaposlenega v AD in storitev vrne kodo napake, ki označuje podvojene ciljne vnose za isti izvorni vnos.

Če želite pregledati dnevnike za enega uporabnika in skupine, glejte Pregled dnevnikov omogočanja uporabe za [težavo z določenim uporabnikom.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
