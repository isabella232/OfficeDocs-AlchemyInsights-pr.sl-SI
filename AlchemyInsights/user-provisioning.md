---
title: Omogočanje uporabe uporabnika
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482915"
---
# <a name="user-provisioning"></a>Omogočanje uporabe uporabnika

- S funkcijo za [Omogočanje uporabe na zahtevo](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) lahko uporabniku zagotovite podrobno diagnostiko o sprejetih korakih.
- Če želite odpraviti težave, s katerimi se srečujete pri omogočanju uporabe uporabnikov in skupin, glejte vodnik za odpravljanje težav [brez uporabe uporabnikov](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Če opazite, da uporabniki niso omogočeni, glejte [Omogočanje dnevnikov (predogled)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) v storitvi Azure Active Directory (ad). Poiščite vnose dnevnika, ki se nanašajo na določenega uporabnika.
- Občasno znova zaženite omogočanje uporabe, da ujamete vse uporabnike, ki so bili zamujeni v prejšnjem ciklu za omogočanje uporabe.
- Uporabnik/skupina morda ni bila omogočena, ker naša storitev še ni imela možnosti, da bi ocenila uporabnika. Preglejte navodila o tem, kako dolgo omogoča omogočanje uporabe, kot tudi vrstico napredovanja na strani s konfiguracijo za omogočanje uporabe. Če je stanje stalnega stanja, ki je določeno v razdelku dodatne podrobnosti, pred datumom, ko je bil uporabnik ustvarjen/posodobljen/izbrisan, to pomeni, da še nismo ocenili uporabnika. V tem primeru je najbolje, da počakate, da se storitev za omogočanje uporabe dokonča. Če je bil dosežen stalen stanje, vam priporočamo, da znova zaženete sistem uporabniškega vmesnika v portalu Azure.
  - Upoštevajte, da je naša storitev seznanjena le s spremembami uporabnika/skupine v izvornem sistemu (Azure Active Directory). Če je uporabnik/skupina odstranjen neposredno v aplikaciji (na primer ServiceNow), ne poznamo teh sprememb in jih ne obračamo na podlagi stanja uporabnika v izvornem sistemu. V tem primeru je najbolje, da znova razveljavite spremembo v ciljnem programu.
- Naša storitev je ocenila uporabnika/skupino in jo določila, da ne sme biti omogočena:
  - Če ste nastavili obseg za dodeljene uporabnike in skupine, preverite, ali je uporabnik/skupina dodeljen programu.
  - Če je uporabniku/skupini dodeljena aplikacija, zagotovite, da niso dodeljena privzeti Accessovi vlogi. Te vloge ni mogoče uporabiti za omogočanje uporabe.
  - Če ste nastavili filter za določanje obsega na osnovi atributa, zagotovite, da uporabnik izpolnjuje pogoje, ki ste jih navedli.
  - Če uporabniki že obstajajo v ciljnem sistemu in stanju uporabnika v izvorni in ciljni tekmi, ne bomo ukrepali.
- Naša storitev je poskušala omogočiti uporabnika in je spodletela. Za te scenarije si oglejte zavihek odpravljanje težav in priporočil v dnevnikih za omogočanje uporabe:
  - Zahtevani atribut uporabnika morda manjka v imeniku Azure Active Directory ali pa se ne ujema z obliko, ki jo zahteva tretja aplikacija. Atribut» država «v uporabniku je lahko na primer nastavljen na Združene države, ko bi moral biti naš.
  - Atribut je referenčni atribut, ki v ciljnem programu še ne obstaja. Referenčni atribut je atribut, ki kaže na drug predmet, na primer uporabnika, ki je član skupine. ID uporabnika bi bil v atributu» član «skupine, vendar ga je mogoče obdelati le, če uporabnik nasprotuje temu, da že obstaja.
