---
title: Napaka Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903128"
---
# <a name="winsock-error-10061"></a>Napaka Winsock 10061

Pomeni ta koda napake, da Office 365 ni mogel vzpostaviti vtičnico TCP (povezava) s ciljnega gostitelja. Najverjetnejši vzrok te napake je problem s konfiguracijo požarnega zidu. Težavo, preverite te nastavitve:
  
- Preverite konfiguracijo požarnega zidu z informacijami v [Office 365 URL in IP naslov razponi](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Če napaka je specifična za Exchange Online varstvo (EOP), si mora prej vročenega spremembo v [Exchange Online zaščite IP naslove](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Preverite, da vaš Internet storitev ponudnik (ISP) ni blokira vrata.
    
- Preverjanje pametnih in gostiteljskim ter ciljnim nastavitve strežnika v vaš priključki.
    
Upoštevajte, da Office 365 ne blokira *dohodne* povezave na ta način. 
  

