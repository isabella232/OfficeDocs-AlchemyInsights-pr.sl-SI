---
title: 1065 zastaranje EOP odhodnega IP naslova rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806811"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Zastaranje EOP odhodnih naslovov IP

Zaznali smo potencialno težavo z vašo organizacijo, ki (če ni popravljena do oktobra 26. oktober 2018), lahko prelom pošte prekine s storitvijo na mestu uporabe ali zunanjimi cilji. Kot je bilo predhodno sporočeno, da poenostavite upravljanje obsega naslovov IP, združujemo obsege naslovov IP za Exchange Online (EOP), ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj programa Microsoft 365. Naša analiza kaže, da je eden ali več zunanjih virov e-pošte ali ciljev, ki ste jih konfigurirali v povezovalnikih toka pošte, ne sprejema povezav z [prikazanih](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)obsegov naslovov IP.

Ukrepajte pred oktobrom 26, da zagotovite, da bodo ti viri in cilji sprejeli povezave do vseh [objavljenih EOP naslovov IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)in iz njih.

Če želite več informacij o tej spremembi, glejte sporočila središča za pošto [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Opomba**: Če ste že uporabljali IP ali URL za objavljanje prek storitev HTML, XML in RSS za končne točke, morate preseliti tudi v nove spletne storitve za avtomatizacijo teh vrst posodobitev. Če želite več informacij, glejte [kategorije končnih točk za microsoft 365 in microsoft 365 naslov IP ter spletna storitev URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
