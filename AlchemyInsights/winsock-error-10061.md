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
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859156"
---
# <a name="winsock-error-10061"></a>Napaka Winsock 10061

Pomeni ta koda napake, da Office 365 ni mogel vzpostaviti vtičnico TCP (povezava) s ciljnega gostitelja. Najverjetnejši vzrok te napake je problem s konfiguracijo požarnega zidu. Težavo, preverite te nastavitve:

- Preverite konfiguracijo požarnega zidu z informacijami v [Office 365 URL in IP naslov razponi](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Če napaka je specifična za Exchange Online varstvo (EOP), si mora prej vročenega spremembo v [Exchange Online zaščite IP naslove](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Preverite, da vaš Internet storitev ponudnik (ISP) ni blokira vrata.

- Preverjanje pametnih in gostiteljskim ter ciljnim nastavitve strežnika v vaš priključki.

Upoštevajte, da Office 365 ne blokira *dohodne* povezave na ta način.
