---
title: Ustvarjanje mesta v storitvi SharePoint online
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
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732256"
---
# <a name="create-sharepoint-sites-using-templates"></a>Ustvarjanje SharePointovih mest s predlogami

Možnost shranjevanja mesta kot predloge ni podprta s sodobnimi komunikacijskimi ali spletnimi mesti skupine. Če želite več informacij o uporabi predlog [, glejte shranjevanje, prenos in prenos SharePointovega mesta kot predloge](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tukaj je nekaj pogostih težav/rešitev glede shranjevanja mesta ali seznama kot predloge v SharePoint Onlineu. 

**Gumb» Shrani spletno mesto/seznam «ni na voljo ali manjka**

Skrbniki bodo morali omogočiti skript po meri, če želite omogočiti funkcije predloge. Za podrobne korake, primere in premisleke glejte 

- [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Ukaz» Shrani mesto kot predlogo «ni podprt in lahko povzroči težave na mestih, ki uporabljajo SharePoint Server Publishing Infrastructure.

**Predloge mesta ni mogoče ustvariti ali pa ne deluje pravilno**

Predloga morda manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in ne bo aktivirana. Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predloge mesta za ustvarjanje spletnega mesta.

- Preverite, ali kateri koli seznami ali knjižnice presegajo [mejni prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) v 5000 elementih, saj lahko to blokira ustvarjanje predloge mesta.

- Mesto lahko uporablja preveč virov in zato predloga mesta presega omejitev 50 MB.


- Na voljo so težave s prikazom podatkov s seznama, ki uporablja stolpec za iskanje. Če želite več informacij, glejte [seznam ustvarjenih predlog ne prikazuje podatkov s pravilnega seznama za iskanje v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Če želite podrobnejše informacije o pogostih težavah in rešitvah, glejte [Ustvarjanje in uporaba predlog spletnega mesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



