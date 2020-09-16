---
title: 'AIP: pravilniki, ki se ne obnašajo po pričakovanjih'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663205"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: pravilniki, ki se ne obnašajo po pričakovanjih

Zaščita informacij Azure: pravilniki, ki se ne obnašajo po pričakovanjih, si oglejte navodila za priporočene smernice za različne težave pravilnika:

1. Če imate težave z vizualnimi oznakami, si oglejte, [Kdaj se izvajajo vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Če imate težave s samodejnim označevanjem, si oglejte [navodila za konfiguracijo pogojev za samodejno in priporočeno razvrstitev za zaščito informacij](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) v storitvi Azure in informacije, [ki jih](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)iščejo.
3. Če imate težave s storitvijo native/Pfile Protection, preberite [Konfiguracija datoteke API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Preverite, ali uporabljate pravilnike o obsegu, ki niso pravilno konfigurirani: [kako konfigurirati pravilnik o varstvu informacij Azure za določene uporabnike z uporabo pravilnikov o obsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Če Samodejna oznaka za Outlook ne deluje v Outlooku, ko priložite označen dokument, preverite, ali DRMEncryptProperty ni opredeljen, kot je opisano tukaj: [nastavitve registra IRM za varnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Če še vedno prihaja do težav, si oglejte dnevnike odjemalca za zaščito informacij Azure in priložite izvožene dnevnike tej vstopnici.

1. Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v Outlooku.
2. Kliknite pomoč za **zaščito/občutljivost**  >  **in povratne informacije**.
3. Kliknite **Izvozi dnevnike**.
4. Shranite dnevnike na izbrano mesto in jih priložite na to zahtevo storitve.

Dodatni viri:

- [Konfiguracija oznake za vizualne oznake za zaščito informacij v storitvi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pregled dokumentacije za zaščito informacij Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Uporaba oznak občutljivosti v aplikacijah Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

