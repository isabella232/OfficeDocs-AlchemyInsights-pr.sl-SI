---
title: Napaka 1554 Winsock 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698878"
---
# <a name="winsock-error-10061"></a>Napaka Winsock 10061

Ta koda napake pomeni, da Microsoft ni mogel vzpostaviti TCP vtičnice (povezave) s ciljnim gostiteljem. Najverjetnejši vzrok te napake je težava pri konfiguraciji požarnega zidu. Težavo odpravite tako, da preverite te nastavitve:

- Preverjanje konfiguracije požarnega zidu s podatki v [URL-jih naslovov Microsoft 365 in obsegi naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Če je prišlo do napake v storitvi Exchange Online Protection (EOP), bi morali biti predhodno obveščeni na spremembo [naslovov IP za Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Preverite, ali vaš ponudnik internetnih storitev (ISP) ne blokira vrat.

- Preverite nastavitve pametnega gostitelja in ciljnega strežnika v povezovalnikih.

Upoštevajte, da Microsoft 365 ne blokira *dohodnih* povezav na ta način.
