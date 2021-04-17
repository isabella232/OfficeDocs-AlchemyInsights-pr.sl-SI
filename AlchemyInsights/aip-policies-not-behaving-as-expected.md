---
title: 'AIP: Pravilniki se ne poshajo po pričakovanjih'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821643"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Pravilniki se ne poshajo po pričakovanjih

Azure Information Protection: Pravilniki se ne obnašajo po pričakovanjih. Če želite priporočene smernice za različne težave s pravilnikom, glejte te smernice:

1. Če imate težave z vizualnimi oznakami, preglejte [Ko uporabite vizualne oznake.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Če imate težave s samodejnim označevanjem, preberite Konfiguracija pogojev za samodejno in priporočeno razvrstitev za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) in Kaj so vrste občutljivih [informacij.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Če imate težave z izvorno zaščito/zaščito datoteke Pfile, preglejte Konfiguracija [API-ja datoteke.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Preverite, ali uporabljate pravilnike z obsegi, ki niso pravilno konfigurirani: Kako konfigurirati pravilnik Azure Information Protection za določene uporabnike z [uporabo pravilnikov o obsegu.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Če samodejno označevanje ne deluje v Outlooku, ko priložite označen dokument, se prepričajte, da DRMEncryptProperty ni definiran tako, kot je opisano tukaj: Nastavitve registra upravljanja pravic do informacij za [varnost.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Če še vedno prihaja do težav, zberite dnevnike odjemalcev za Azure Information Protection in priložite izvožene dnevnike tej vstopnici.

1. Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v Outlooku.
2. Kliknite **Pomoč za zaščito/občutljivost**  >  **in povratne informacije.**
3. Kliknite **Izvoz dnevnikov.**
4. Shranite dnevnike v svojo izbiro lokacije in jih priložite tej zahtevi za storitev.

Dodatni viri:

- [Konfiguracija oznake za vizualne oznake za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pregled dokumentacije Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Uporaba oznak občutljivosti v aplikacijah Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

