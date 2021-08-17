---
title: 1554 Obok 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083246"
---
# <a name="winsock-error-10061"></a>Napaka Obok 10061

Ta koda napake pomeni, da Microsoft ni mogel vzpostaviti vtičnice TCP (povezave) s ciljnim gostiteljem. Najverjetnejši vzrok za to napako je težava v konfiguraciji požarnega zidu. Če želite odpraviti težavo, preverite te nastavitve:

- Preverjanje konfiguracije požarnega zidu z informacijami [Microsoft 365 URL-jih](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) in obsegih naslovov IP

- Če je napaka specifična za Exchange Online Protection (EOP), bi morali biti prej obveščeni o spremembi [naslovov IP za Exchange Online Protection IP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Prepričajte se, da ponudnik internetnih storitev (ISP) ne blokira vrat.

- Preverite nastavitve pametnega gostitelja in ciljnega strežnika v povezovalnikih.

Upoštevajte, Microsoft 365 ta ne blokira *dohodnih* povezav.
