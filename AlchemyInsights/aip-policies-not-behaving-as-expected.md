---
title: 'AIP: politike, ki se ne obnaša po pričakovanjih'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506574"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politike, ki se ne obnaša po pričakovanjih

Azure Information Protection: pravilniki se ne obnaša po pričakovanjih, za priporočene smernice za različna politična vprašanja glejte naslednje:

1. Če imate težave z vizualnimi oznakami, preglejte, [Kdaj se uporabljajo vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Če imate težave z avtomatskim označevanjem, preglejte, [Kako konfigurirate pogoje za samodejno in priporočeno razvrščanje za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) in [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Če imate težave z native/Pfile zaščito, prosimo, preglejte [datoteko API konfiguracijo](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Preverite, ali uporabljate pravilnike v obsegu, ki niso pravilno konfigurirani: [kako konfigurirati pravilnik o varstvu podatkov Azure za določene uporabnike z uporabo pravilnikov v obsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Če samodejno označevanje ne deluje v Outlooku, ko pripnete označeni dokument, preverite, ali DRMEncryptProperty ni definiran, kot je opisano tukaj: [nastavitve registra IRM za varnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Če še vedno naletite na težave, prosimo, zberite Azure Information Protection dnevniki in priložite izvožene dnevnike na to vozovnico.

1. Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v programu Outlook.
2. Kliknite **zaščitite/občutljivost**  >  **pomoč in povratne informacije**.
3. Kliknite **Izvozi dnevnike**.
4. Shranite dnevnike na svojo izbiro lokacije in jih priložite tej zahtevi za storitev.

Dodatni viri:

- [Konfiguriranje oznake za vizualne oznake za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Preglejte dokumentacijo o varstvu podatkov Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Uporaba oznak občutljivosti v Officeovih aplikacijah](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

