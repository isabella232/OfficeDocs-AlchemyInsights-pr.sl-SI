---
title: DLP ne deluje po pričakovanjih
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932638"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne deluje po pričakovanjih

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

 **Nastavitev DLP**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** v officeu 365 ne deluje po pričakovanjih? Če je tako, se prepričajte, da je **pravilnik DLP** pravilno nastavljen in da podatki vsebujejo tisto, kar išče **pravilnik DLP** , ko se ovrednoti.
  
Pravilniki DLP omogočajo prepoznavanje in zaščito občutljivih informacij v organizaciji. Če želite nastaviti pravilnike DLP, uporabite informacije [tukaj](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Katere politike DLP iščejo**
  
Pri uporabi **vgrajenih občutljivih vrst informacij** v središču Office 365 varnost in skladnost center, pravilniki DLP pri odkrivanju teh občutljivih tipov iščejo določene vzorce in elemente.
  
- **Vgrajene vrste občutljivih informacij**

    Če želite več informacij o vgrajenih vrstah občutljivih in o tem, kaj je videti v pravilniku o DLP pri odkrivanju občutljive vrste, glejte: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Vrste občutljivih informacij po meri**

    Če poskušate ustvariti občutljive vrste informacij po meri, uporabite ta članek za informacije o tem, kako ustvariti občutljivo vrsto po meri: [ustvarite vrsto občutljive informacije po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Preskusite pravilnik DLP**

Če želite podatke preskusiti z vgrajenim ali po meri občutljivim informacijskim tipom, uporabite možnost **Vrsta preskusa** pod **razvrstitvami** > **občutljivih vrst**informacij. Če želite več informacij, glejte [preizkušanje občutljivih vrst informacij po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Poročila**
  
- Pridobite občutljive vpoglede podatkov s [poročili DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Oglejte si posebne podrobnosti dogodka s [poročilom o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
