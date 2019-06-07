---
title: 1065 Negodovanje EOP odhodne IP naslov rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752971"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Negodovanje EOP odhodne IP naslov razponi

Smo odkrili do morebitnega vprašanje z organizacijo, ki (če ni popravljen s oktober 26, 2018) morda prekinil tok pošte krajevne ali zunanjih ciljev. Kot prej sporočiti, poenostaviti upravljanje IP naslov obsega, smo si utrditev Exchange Online varstvo (EOP) IP naslov območja, ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj Office 365. Naše analize kažejo, da eden ali več zunanjih email virov ali ciljev, ki ste jih konfigurirali v poštni tok priključki niso sprejemanje povezav iz je IP naslov razponi prikazano [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Delovala pred 26 oktobra za zagotovitev teh virov in destinacij bo sprejemanje povezav in iz vseh [objavljenih EOP IP naslove](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Če želite več informacij o tej spremembi, si oglejte sporočilo Center delovnih mest, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Opomba**: Če ste prej uporabljali IP ali URL objavljanje preko HTML, XML in RSS za posodobitve končna točka, tudi naj preselite v novih spletnih storitev za avtomatizacijo tovrstnih posodobitve. Če želite več informacij, glejte [Office 365 končne točke kategorije in Office 365 IP naslov in spletni naslov spletne storitve](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
