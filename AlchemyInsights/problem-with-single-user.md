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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430207"
---
# <a name="problem-with-single-user"></a>Težava z enim uporabnikom

- Uporabnik morda ni bil omogočen, ker storitev še ni imela možnosti, da bi ocenila uporabnika. Preglejte navodila o tem, kako dolgo omogoča omogočanje uporabe, kot tudi vrstico napredovanja na strani s konfiguracijo za omogočanje uporabe. Če je stanje stalnega stanja, ki je določeno v razdelku dodatne podrobnosti, pred datumom, ko je bil uporabnik ustvarjen/posodobljen/izbrisan, to pomeni, da še nismo ocenili uporabnika. V tem primeru je najbolje, da počakate, da se storitev za omogočanje uporabe dokonča.

  - Upoštevajte, da je naša storitev seznanjena le s spremembami uporabnika v izvornem sistemu (v oblaku). Obstajati mora veljavna sprememba v izvornem sistemu za Azure AD, da zazna spremembo in jo poteče v imenik Active Directory.
- Storitev za omogočanje uporabe je ocenila uporabnika in ga določila, da ne sme biti omogočena:
  - Če ste nastavili filter za določanje obsega na osnovi atributa, zagotovite, da uporabnik izpolnjuje pogoje, ki ste jih navedli.
  - Če uporabniki že obstajajo v ciljnem sistemu in stanju uporabnika v izvorni in ciljni tekmi, ne bomo ukrepali.
- Storitev za omogočanje uporabe je poskušala omogočiti uporabnika in je spodletela. Za te scenarije si oglejte zavihek odpravljanje težav in priporočil v dnevnikih za omogočanje uporabe:
  - Zahtevani atribut uporabnika morda manjka v imeniku Active Directory na mestu uporabe ali v storitvi Azure AD. Na primer pravila userPrincipalName ali sAMAccountName generacije ne ustvarijo prave vrednosti.
  - Ujemajoči se atribut (običajno IDZaposlenega) ne razreši enoličnemu uporabniku v imeniku Active Directory na mestu uporabe ali v storitvi Azure AD. Na primer obstajata dva uporabnika z istim IDZaposlenega v storitvi AD in storitev vrne kodo napake, ki označuje podvojene ciljne vnose za isti izvorni vnos.

Če želite pregledati dnevnike za enega uporabnika in skupine, si oglejte [pregled dnevnikov za omogočanje težave z določenim uporabnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
