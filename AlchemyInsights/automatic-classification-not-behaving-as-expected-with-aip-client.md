---
title: Samodejna razvrstitev z odjemalcem AIP se ne obnaša po pričakovanjih
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820914"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Samodejna razvrstitev z odjemalcem AIP se ne obnaša po pričakovanjih

Če se samodejna klasifikacija ne obnaša po pričakovanjih, uporabite naslednje priporočene smernice:

1. Če imate težave s samodejnim označevanjem, glejte [Kako konfigurirati pogoje za samodejno in priporočeno razvrstitev za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) in [Kaj se išče z vrstami občutljivih informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Preverite, ali uporabljate pravilnike z obsegom, ki niso pravilno konfigurirani: [Kako konfigurirati pravilnik storitve Azure Information Protection s pravilniki z obsegom za določene uporabnike](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Če samodejno označevanje za Outlook ne deluje, ko priložite označen dokument, se prepričajte, da `DRMEncryptProperty` ni definiran tako, kot je opisano tukaj: [nastavitve registra IRM za varnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Če ste za pravilnik Azure Information Protection uporabili [vgrajene vrste informacij](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b), preverite, ali se vsebina ujema s pričakovano obliko zapisa.
5. Preverite, ali je oznaka ustrezno konfigurirana za **Samodejno** ali **Priporočeno**. (**Samodejno** označevanje je na voljo za vse aplikacije Microsoft 365, medtem ko je **Priporočeno** na voljo za vse aplikacije Microsoft 365 razen za Outlook.)
6. Samodejne razvrstitve ne morete uporabiti za dokumente in e-poštna sporočila, ki so bila prej ročno označena ali samodejno označena z višjo stopnjo razvrstitve.  Če želite več informacij, glejte: [Kako so uporabljene samodejne ali priporočene oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Če še vedno prihaja do težave, zberite dnevnike odjemalcev za Azure Information Protection in vstopnici za podporo priložite izvožene dnevnike. Če želite izvoziti dnevnike storitve Azure Information Protection:
    - Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v Outlooku.
    - Kliknite pomoč za **zaščito/občutljivost** > **povratne informacije**.
    - Kliknite **izvoz dnevnikov**.
    - Shranite dnevnike na svojo lokacijo in jih priložite zahtevi za storitev.

Če želite več informacij, glejte:

- [Konfiguracija pogojev za samodejno in priporočeno razvrstitev za storitev Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Vodniki z navodili za pogoste scenarije, ki uporabljajo storitev Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Pregled dokumentacije za storitev Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pregled naročnin in funkcij storitve Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Zahteve za storitev Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Vadnica za hitri začetek s storitvijo Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Prenos odjemalca storitve Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
