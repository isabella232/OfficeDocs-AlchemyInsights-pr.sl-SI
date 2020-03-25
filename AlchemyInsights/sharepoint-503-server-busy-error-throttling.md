---
title: SharePoint online Throttling
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931242"
---
# <a name="sharepoint-online-throttling"></a>SharePoint online Throttling

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

**503 strežnik je zaseden napaka**

Uporabnik maj sprejemati a 503 pomočnik je zaposlen zmota čas poskus v pluti v SharePoint ali OneDrive položaj. 

To napako lahko povzroči zadavljenje znotraj storitve SharePoint. SharePoint online uporablja zadaviti za ohranjanje optimalne učinkovitosti in zanesljivosti storitve SharePoint online. Throttling omejuje število uporabniških dejanj ali sočasnih klicev (po skriptu ali kodi), da se prepreči prekomerna uporaba virov. 

Za več informacij o zadaviti glej, [ne pridobivanje zadaviti ali blokiran v SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Če menite, da ta napaka ni povezana z Throttling, lahko preverite, ali je aktivno vzdrževanje, ki se pojavljajo na vašem najemniku z navigacijo do [centra za sporočila](https://portal.office.com/adminportal/home#/MessageCenter).

 Slednjič, zavarovati vi kratek obisk [usluga zdravje](https://portal.office.com/adminportal/home#/servicehealth) stran v ček zakaj poljuben Advisories/nezgoda to maj obstati dogodek.

