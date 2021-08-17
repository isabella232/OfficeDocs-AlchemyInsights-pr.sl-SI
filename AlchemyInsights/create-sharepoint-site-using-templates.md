---
title: Ustvarjanje spletnega mesta v SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057982"
---
# <a name="create-sharepoint-sites-using-templates"></a>Ustvarjanje SharePoint mest s predlogami

Sodobna spletna mesta za komunikacijo ali skupino ne podpirajo možnosti shranjevanja spletnega mesta kot predloge. Če želite več informacij o uporabi predlog mest, glejte [Shranite, prenesite in naložite mesto programa SharePoint kot predlogo](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tukaj je nekaj pogostih težav/rešitev v zvezi s shranjevanjem mesta ali seznama kot predloge v SharePoint Onlineu. 

**Save site/list template button is not available or missing**

Skrbniki bodo morali omogočiti skript po meri, da omogočijo funkcije predloge. Če želite podrobna navodila, si oglejte primere in pomisleke. 

- [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Ukaz Shrani mesto kot predlogo ni podprt in lahko povzroči težave na mestih, ki uporabljajo infrastrukturo strežnika SharePoint Server za objavljanje.

**Predloge mesta ni mogoče ustvariti ali ne deluje pravilno**

V predlogi morda manjka funkcija [in je](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ni mogoče aktivirati. Če funkcije ni mogoče aktivirati v trenutni zbirki spletnih mest, ne morete uporabiti predloge mesta za ustvarjanje mesta.

- Preverite, ali kateri od seznamov oz. knjižnic presega [Prag omejitve za pogled seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), ki je nastavljen na 5000 elementov. Presežen prag lahko blokira ustvarjanje predloge mesta.

- Spletno mesto morda uporablja preveč virov, zato predloga spletnega mesta presega omejitev 50 MB.


- Pri prikazu podatkov s seznama, ki uporablja stolpec za iskanje, je prišlo do težav Če želite več informacij, si oglejte [Seznam, ustvarjen s predlogo, ne prikazuje podatkov s pravilnega seznama za iskanje v storitvi SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Če želite podrobnejše informacije o pogostih težavah in rešitvah, [si oglejte Ustvarjanje in uporaba predlog mest.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



