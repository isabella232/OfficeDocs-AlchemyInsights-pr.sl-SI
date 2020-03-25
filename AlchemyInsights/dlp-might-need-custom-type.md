---
title: DLP bo morda potreboval vrsto po meri
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932674"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP bo morda potreboval vrsto po meri

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

**DLP lahko zahteva vrsto informacij po meri**

S pravilnikom za preprečevanje izgub podatkov (DLP) lahko prepoznate in zaščitite občutljive podatke v organizaciji. V nekaterih primerih boste morda morali ustvariti lastne občutljive vrste podatkov **po meri** za zaščito podatkov organizacije.

Vaša organizacija bo morda morala na primer identificirati in zaščititi ID-je zaposlenih ali druge podatke v neki obliki, ki je specifična za vašo org. Če je tako, si oglejte naslednje članke za več informacij.
  
 **Prilagajanje vgrajene občutljive vrste informacij**
  
Če bi vgrajena vrsta občutljivih informacij zadovoljila vaše potrebe s samo nekaj poteg, lahko [prilagodite vgrajeno vrsto občutljivih podatkov](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Dodajate ali odstranjujete lahko na primer ključne besede ali dodajate ali odstranjujete dokazila, kot sta datum ali naslov.
  
 **Ustvarjanje vrste občutljivih podatkov po meri**
  
Če pa morate v celoti prepoznati in zaščititi drugačno vrsto občutljivih informacij, lahko [ustvarite vrsto občutljive informacije po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) v uporabniškem vmesniku varnostnega & središča za skladnost.
  
**Ustvarjanje občutljive vrste podatkov po meri v varnostnem & PowerShell center za skladnost**

Končno, če UI ne zagotavlja vseh možnosti, ki jih potrebujete, lahko [ustvarite po meri občutljive informacije vrsto v Security & skladnost center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Z začetkom z datoteko XML lahko uporabite vse razpoložljive možnosti.
