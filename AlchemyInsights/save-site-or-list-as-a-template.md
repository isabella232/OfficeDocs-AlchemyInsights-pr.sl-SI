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
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727547"
---
# <a name="save-site-or-list-as-a-template"></a>Shranjevanje mesta ali seznama kot predloge

Predloge SharePointovih mest so vnaprej ustvarjene definicije, oblikovane okoli določene poslovne potrebe. Če želite več informacij, glejte [Uporaba predlog za ustvarjanje različnih vrst SharePointovih mest](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tukaj je nekaj pogostih težav/rešitev glede shranjevanja mesta ali seznama kot predloge v SharePoint Onlineu.

**Gumb» Shrani mesto/seznam «ni na voljo ali manjka**. 

- Skrbniki bodo morali omogočiti skript po meri, če želite omogočiti funkcije predloge. Če želite podrobna navodila, primeri in premisleki, glejte [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Ukaz» Shrani mesto kot predlogo «ni podprt in lahko povzroči težave na mestih, ki uporabljajo SharePoint Server Publishing Infrastructure.


**Predloge mesta ni mogoče ustvariti ali pa ne deluje pravilno**

- Predloga morda manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in ne bo aktivirana. Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predloge mesta za ustvarjanje spletnega mesta.


- Preverite, ali kateri koli seznami ali knjižnice presegajo [mejni prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) v 5000 elementih, saj lahko to blokira ustvarjanje predloge mesta.


- Mesto lahko uporablja preveč virov in zato predloga mesta presega omejitev 50 megabajtov (MB).


- Na voljo so težave s prikazom podatkov s seznama, ki uporablja stolpec za iskanje. Če želite več informacij, glejte [seznam ustvarjenih predlog ne prikazuje podatkov s pravilnega seznama za iskanje v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Če želite podrobnejše informacije o pogostih težavah in rešitvah, se lahko sklicujete na [Ustvarjanje in uporabo predlog spletnega mesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

