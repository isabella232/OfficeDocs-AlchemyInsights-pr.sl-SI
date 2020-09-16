---
title: Težave z učinkovitostjo delovanja – SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771917"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ali OneDrive počasno, nedostopno ali ni na voljo za več uporabnikov

SharePoint ali OneDrive je lahko počasno, nedostopno ali pa ni na voljo ali pa lahko prikaže storitev nedostopnih ali 503, iz več razlogov:
  
- Če je SharePointovo ali OneDrive mesto počasno ali Zakasnjeno za več uporabnikov, je morda prišlo do začasne težave s storitvijo, kjer uporabniki občasno opazijo ponavljajoče se zamude ali napake pri krmarjenju, ko dostopajo do SharePointovih mest ali vsebine OneDrive. Preverite, ali je [Nadzorna plošča za zdravstveno stanje na voljo](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , če želite preveriti, ali je vaša organizacija vplivala nanje.
  
- Uporabniki lahko prejmejo *strežnik 503,* ko poskušate krmariti do SharePointovih mest ali OneDrive. Do te napake lahko pride zaradi omejevanja v SharePointovi storitvi. Storitev SharePoint Online z omejevanjem zmogljivosti vzdržuje optimalno učinkovitost in zanesljivost storitve SharePoint Online. Omejevanje zmogljivosti omeji število uporabniških dejanj ali sočasnih klicev (s skriptom ali kodo) in tako prepreči prekomerno uporabo sredstev. Če želite več informacij o omejevanju prikaza, [preprečite, da bi se v SharePoint onlineu izognili omejevanju ali blokiranju](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Če imate počasno učinkovitost delovanja s **klasičnim** ali **sodobnim** SharePointovim mestom ali stranjo, uporabite [diagnostično orodje](https://aka.ms/perftool) za analizo strani.
  
- Če še vedno uporabljate splošno počasno učinkovitost delovanja, si oglejte vire na dnu tega članka: [Uvod v prilagajanje učinkovitosti delovanja za SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  