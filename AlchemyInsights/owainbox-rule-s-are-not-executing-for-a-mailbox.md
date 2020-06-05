---
title: 1332 OWA-Prejeto pravilo (e) se ne izvaja za nabiralnik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576576"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo» Prejeto «ne deluje po pričakovanjih

Preverite naslednje nastavitve v programu Outlook v spletu:

- Sporočilo se lahko preusmeri, posreduje ali odgovori samodejno na podlagi pravil» Prejeto «samo enkrat. Pravilo za preusmerjanje (pravilo» Prejeto «ali pravilo toka pošte, znano tudi kot pravilo prenosa) lahko sporočilu doda največ deset prejemnikov za posredovanje. Če želite več informacij, glejte [omejitve pravil temeljnice, transporta in nabiralnika](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravila nabiralnika ne delujejo v nabiralniku nadomestnega dnevnika. Če želite več informacij o nadomestnem nabiralniku za dnevnike, glejte [nadomestni dnevniki za journaling](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Če želite odpraviti ta vprašanja, glejte [KB 2829319](https://support.microsoft.com/kb/2829319).

Če prejšnja vprašanja ne veljajo, zaženite diagnostično poročilo pravila za Inbox, preden težavo še stopnjevate z Microsoftovo podporo:

1. Odprite nabiralnik v programu Outlook v spletu in kliknite <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavitvami**  >  **Oglejte si vse nastavitve Outlook**  >  **Pošte**  >  **Pravila**.

2. Na dnu strani kliknite, **Če vaša pravila ne delujejo, kliknite tukaj, če želite ustvariti diagnostično poročilo**.
