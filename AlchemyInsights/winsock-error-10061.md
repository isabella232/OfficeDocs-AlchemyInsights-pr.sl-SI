---
title: 1554 Winsock napaka 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766185"
---
# <a name="winsock-error-10061"></a>Winsock napaka 10061

Ta koda napake pomeni, da Microsoft ni mogel vzpostaviti TCP vtičnice (povezave) s ciljnim gostiteljem. Najverjetnejši vzrok za to napako je težava s konfiguracijo požarnega zidu. Težavo odpravite tako, da preverite te nastavitve:

- Preverite konfiguracijo požarnega zidu z informacijami v [Microsoft 365 URL-jev in obsegih IP naslovov](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Če je napaka specifična za spletno zaščito Exchange Online (EOP), bi morali biti prej obveščeni o spremembi [naslovov IP za zaščito Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Preverite, ali ponudnik internetnih storitev (ISP) ne blokira vrat.

- Preverite nastavitve pametnega gostitelja in ciljnega strežnika v konektorjih.

Upoštevajte, da Microsoft 365 ne blokira *dohodnih* povezav na ta način.
