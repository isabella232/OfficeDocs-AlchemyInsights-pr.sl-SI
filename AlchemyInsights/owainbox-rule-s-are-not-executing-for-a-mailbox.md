---
title: 1332 OWA – pravilo za mapo» Prejeto «se ne izvaja za nabiralnik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721607"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo za mapo» Prejeto «ne deluje po pričakovanjih

V Outlooku v spletu preverite te nastavitve:

- Sporočilo lahko preusmerite, posredujete ali odgovorite samodejno na podlagi pravil za mapo» Prejeto «le enkrat. Pravilo za preusmerjanje (pravilo za mapo» Prejeto «ali pravilo za prenos pošte, znano tudi kot pravilo prenosa) lahko v sporočilo doda največ deset prejemnikov. Če želite več informacij, glejte [omejitve pravilnika dnevnika, transporta in mape» Prejeto «](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravila za mapo» Prejeto «ne delujejo v drugem nabiralniku dnevnika. Če želite več informacij o nadomestnem nabiralniku temeljnice, glejte [nadomestni nabiralnik v dnevniku](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Če želite odpraviti te težave, glejte [KB 2829319](https://support.microsoft.com/kb/2829319).

Če prejšnje težave ne veljajo, zaženite diagnostično poročilo pravilo za mapo» Prejeto «, preden razširite težavo v Microsoftovo podporo:

1. Odprite nabiralnik v programu Outlook v spletu in kliknite <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavitve**  >  **Ogled vseh Outlookovih nastavitev**  >  **Pošta**  >  **Pravil**.

2. Na dnu strani kliknite, **Če vaša pravila ne delujejo, kliknite tukaj, če želite ustvariti diagnostično poročilo**.
