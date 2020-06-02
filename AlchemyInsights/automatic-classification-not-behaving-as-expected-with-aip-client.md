---
title: Samodejna razvrstitev se ne obnaša po pričakovanjih s stranko AIP
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
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493436"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Samodejna razvrstitev se ne obnaša po pričakovanjih s stranko AIP

Samodejna razvrstitev se ne obnaša po pričakovanjih, uporabite naslednje priporočene smernice:

1. Če imate težave z avtomatskim označevanjem, glejte [kako konfigurirati pogoje za samodejno in priporočeno razvrstitev za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) in [katere vrste občutljivih informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Preverite, ali uporabljate pravilnike v obsegu, ki niso pravilno konfigurirani: [kako konfigurirati pravilnik o varstvu podatkov Azure za določene uporabnike z uporabo pravilnikov v obsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Če samodejno označevanje ne deluje v Outlooku pri prilaganju označenega dokumenta, preverite, `DRMEncryptProperty` ali ni definirano, kot je opisano tukaj: [nastavitve registra IRM za varnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Če ste uporabili [vgrajene vrste informacij](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) za pravilnik o varstvu podatkov Azure, preverite, ali se vsebina ujema s pričakovano obliko.
5. Preverite, ali je nalepka ustrezno konfigurirana za **samodejno** ali **priporočeno**. (**Samodejno** označevanje je na voljo za vse Officeove aplikacije, medtem ko je **priporočeno** na voljo za vse Officeove aplikacije, razen za Outlook.)
6. Samodejne razvrstitve ne morete uporabiti za dokumente in e-poštna sporočila, ki so bila prej ročno označena ali že samodejno označena z višjo razvrstitvijo.  Če želite več informacij, glejte: [Kako se uporabljajo samodejne ali priporočene nalepke](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Če še vedno naletite na težave, prosimo, zberite Azure Information Protection dnevniki in priložite izvožene dnevnike na vašo podporo vozovnice. Če želite izvoziti dnevnike varstva podatkov Azure:
    - Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v programu Outlook.
    - Kliknite **zaščitite/občutljivost**  >  **pomoč in povratne informacije**.
    - Kliknite **Izvozi dnevnike**.
    - Shranite dnevnike na svojo izbiro lokacije in jih priložite zahtevi za storitev.

Za dodatne informacije glejte:

- [Konfiguriranje pogojev za samodejno in priporočeno razvrščanje za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Navodila za pogoste scenarije, ki uporabljajo Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Preglejte dokumentacijo o varstvu podatkov Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Preglejte naročnine in funkcije za zaščito podatkov Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Zahteve za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Vodnik za hitri začetek za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Prenesite odjemalca za zaščito podatkov Azure](https://www.microsoft.com/download/details.aspx?id=53018)
