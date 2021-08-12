---
title: Težave z učinkovitostjo SharePoint ali OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911858"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint, OneDrive, nedostopne ali nedostopne za več uporabnikov

SharePoint ali OneDrive so lahko počasne, nedostopne ali niso na voljo ali pa so prikazane napake storitve, ki niso na voljo, ali 503 napak zaradi več razlogov:
  
- Če je SharePoint ali OneDrive mesto počasno ali zakasnjeno za več uporabnikov, lahko pride do začasne težave s storitvijo, pri kateri lahko uporabniki pride do začasnih zakasnitev ali napak pri krmarjenju, ko dostopajo do SharePoint mest ali OneDrive vsebine. Na nadzorni [plošči s stanjem](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) storitve preverite, ali je to vplivalo na vašo organizacijo.
  
- Uporabniki lahko prejmejo napako, da je strežnik *503* zaseden, ko poskušajo SharePoint ali OneDrive mesta. Do te napake lahko pride zaradi zmogljivosti v SharePoint storitve. Storitev SharePoint Online z omejevanjem zmogljivosti vzdržuje optimalno učinkovitost in zanesljivost storitve SharePoint Online. Omejevanje zmogljivosti omeji število uporabniških dejanj ali sočasnih klicev (s skriptom ali kodo) in tako prepreči prekomerno uporabo sredstev. Če želite več informacij o zmogljivostih, glejte Izogibanje dušenje ali [blokiranje v SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Če s klasičnim  ali sodobnim uporabniškim vmesnikom **SharePoint** učinkovitost delovanja, uporabite orodje [Diagnostika](https://aka.ms/perftool) strani za analizo strani.
  
- Če imate še vedno splošno počasno delovanje, si oglejte vire na dnu tega članka: Uvod v izboljšanje učinkovitosti [delovanja za SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  