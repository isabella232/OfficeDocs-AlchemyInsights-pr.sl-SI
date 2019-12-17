---
title: Težave z učinkovitostjo delovanja-SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068434"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ali OneDrive je počasen, nedostopen ali ni na voljo za več uporabnikov

SharePoint ali OneDrive je lahko počasen, nedosegljiv ali na voljo ali pa lahko prikaže storitev, ki ni na voljo, ali 503 napak iz več razlogov:
  
- Če je vaše spletno mesto SharePoint ali OneDrive počasno ali Zakasnjeno za več uporabnikov, lahko pride do začasne težave s storitvijo, kjer uporabniki pri dostopu do SharePointovih mest ali vsebine v storitvi OneDrive izkusijo prekinjene zamude ali napake pri krmarjenju. Če želite preveriti, ali je vaša organizacija vplivala, preverite [nadzorno ploščo storitve](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .
  
- Uporabnik maj sprejemati a *503 pomočnik je zaposlen* zmota čas poskus v pluti v SharePoint ali OneDrive položaj. To napako lahko povzroči zadavljenje znotraj storitve SharePoint. SharePoint online uporablja zadaviti za ohranjanje optimalne učinkovitosti in zanesljivosti storitve SharePoint online. Throttling omejuje število uporabniških dejanj ali sočasnih klicev (po skriptu ali kodi), da se prepreči prekomerna uporaba virov. Za več informacij o zadaviti glej, [ne pridobivanje zadaviti ali blokiran v SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Če doživite počasno delovanje s **klasičnim** ali **modernim** SharePointovim mestom ali stranjo, uporabite [diagnostično orodje](https://aka.ms/perftool) za analizo strani.
  
- Če še vedno doživite splošno počasno delovanje, preglejte vire na dnu tega članka: [Uvod v tuning učinkovitosti za SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  