---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031278"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Zastarelost obsegov odhodnih naslovov IP za EOP

Zaznali smo morebitno težavo z vašo organizacijo, ki (če ni odpravljena do 26. oktobra 2018) lahko prekine tok pošte v prostorih podjetja ali zunanjih ciljih. Kot ste že posredovali, smo zaradi lažjega upravljanja obsega naslovov IP uskladili obsege naslovov IP za Exchange Online Protection (EOP), ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj Microsoft 365. V naši analizi je navedeno, da eden ali več zunanjih e-poštnih virov ali ciljev, ki ste jih konfigurirali v povezovalnikih toka pošte, ne sprejema povezav iz obsegov naslovov IP, prikazanih [tukaj.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Ukrepajte pred 26. oktobrom, da zagotovite, da ti viri in cilji sprejmejo povezave do vseh objavljenih naslovov [IP za EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)in iz njih.

Če želite več informacij o tej spremembi, glejte Objave v središču za sporočila [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Opomba:** Če ste že uporabljali objavljanje NASLOVOV IP ali URL-ja prek HTML-ja, XML-ja in virov RSS za posodobitve končnih točk, morate te vrste posodobitev preseliti tudi v nove spletne storitve. Če želite več informacij, [glejte Microsoft 365 končnih točk in Microsoft 365 naslov IP in spletno storitev URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
