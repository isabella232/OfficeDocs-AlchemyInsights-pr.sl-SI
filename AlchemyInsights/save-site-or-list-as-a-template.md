---
title: Shranjevanje mesta ali seznama kot predloge
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109220"
---
# <a name="save-site-or-list-as-a-template"></a>Shranjevanje mesta ali seznama kot predloge

SharePoint predloge spletnih mest so vnaprej ustvarjene definicije, oblikovane za določene poslovne potrebe. Če želite več informacij, [glejte Uporaba predlog za ustvarjanje različnih vrst SharePoint mest.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Tukaj je nekaj pogostih težav/rešitev v zvezi s shranjevanjem mesta ali seznama kot predloge v programu SharePoint Online.

**Gumb Shrani predlogo mesta/seznama ni na voljo ali ni na voljo.** 

- Skrbniki bodo morali omogočiti skript po meri, da omogočijo funkcije predloge. Če želite podrobna navodila, si oglejte Omogočanje [ali preprečevanje skripta po meri.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Ukaz Shrani mesto kot predlogo ni podprt in lahko povzroči težave na mestih, ki uporabljajo infrastrukturo strežnika SharePoint Server za objavljanje.


**Predloge mesta ni mogoče ustvariti ali ne deluje pravilno**

- V predlogi morda manjka funkcija [in je](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ni mogoče aktivirati. Če funkcije ni mogoče aktivirati v trenutni zbirki spletnih mest, ne morete uporabiti predloge mesta za ustvarjanje mesta.


- Preverite, ali kateri od seznamov oz. knjižnic presega [Prag omejitve za pogled seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), ki je nastavljen na 5000 elementov. Presežen prag lahko blokira ustvarjanje predloge mesta.


- Mesto morda uporablja preveč virov in zato predloga mesta presega omejitev 50 MB.


- Pri prikazu podatkov s seznama, ki uporablja stolpec za iskanje, je prišlo do težav Če želite več informacij, glejte Seznam, ustvarjen s predlogo, ne prikaže podatkov s pravilnega seznama [za iskanje v SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Če želite podrobnejše informacije o pogostih težavah in rešitvah, glejte [Ustvarjanje in uporaba predlog mest.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

