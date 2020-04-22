---
title: 1065 zastaranje odhodnega IP naslova EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704613"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Zastareanje razponov odhodnega IP-naslova EOP

Odkrili smo morebitno težavo z vašo organizacijo, ki bi (če ne bi bila popravljena do 26. oktobra, 2018) morda prekinil pretok pošte v krajevnih ali zunanjih destinacijah. Kot je bilo že sporočeno, da bi poenostavili upravljanje obsega IP naslovov, utrimo obsege IP naslovov za Exchange Online Protection (EOP), ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj Microsofta 365. Naša analiza kaže, da eden ali več zunanjih virov e-pošte ali ciljev, ki ste jih konfigurirali v konektorje za pretok pošte, ne sprejema povezav iz obsegov naslovov IP, prikazanih [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Zakon pred oktobrom 26th za zagotovitev teh virov in destinacij bo sprejela povezave in iz vseh [objavljenih IP naslove EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Če želite več informacij o tej spremembi, glejte sporočila center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Opombe**: Če ste že uporabljali IP ali URL objavljanje prek HTML, XML in RSS za končne posodobitve, morate tudi preseliti v nove spletne storitve za avtomatizacijo teh vrst posodobitev. Če želite več informacij, glejte [kategorije končnih točk microsoft 365 in spletna storitev microsoft 365 IP naslov in URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
