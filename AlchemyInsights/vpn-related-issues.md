---
title: Težave, povezane z omrežjem VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555745"
---
# <a name="vpn-related-issues"></a>Težave, povezane z omrežjem VPN

Uspešna implementacija povezljivosti VPN za odjemalce MDM je odvisna od razporejenega profila, ki pravilno odraža zahteve infrastrukture VPN. Za ustrezne nastavitve odjemalskih platform, ki jih preiskujete, glejte: 

[Nastavitve holografske naprave za Windows 10 in Windows za dodajanje povezav VPN s storitvijo Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Dodajanje nastavitev VPN v napravah s sistemom iOS in iPadOS v storitvi Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Nastavitve naprave Android za konfiguracijo VPN v intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Dodajanje nastavitev VPN v napravah macOS v programu Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Če vaš profil VPN uporablja preverjanje pristnosti na podlagi potrdila, preverite, ali so korenski certifikat in profili potrdila za preverjanje pristnosti odjemalca, povezani s profilom VPN, uspešno uvedeni.

**Pogosta vprašanja**

**V napravo sem poslal profil VPN. Intune kaže, da je bila uspešna, vendar naprava ne vzpostavlja povezave z VPN.**

Uspešno stanje pomeni, da je Intune uspešno uvedel profil kot konfiguriran. Vendar pa te konfiguracije morda ne ustrezajo vašim zahtevam za omrežje in/ali preverjanje pristnosti. Če želite več podrobnosti o poskusu povezave, preglejte dnevnike v infrastrukturi in storitvi za preverjanje pristnosti (v strežniku VPN in strežniku NPS/Radius). Če želite zbirati in pregledovati dnevnike, boste morda morali sodelovati z ekipo za omrežno infrastrukturo ali prodajalcem vpn drugega ponudnika.

**Ko konfiguriram VPN po meri za iOS, funkcija VPN po aplikaciji ni na voljo.**

VPN za aplikacije v omrežju iOS v intunu je trenutno na voljo na določenem seznamu ponudnikov in partnerjev, ki morajo izpolnjevati tudi zahteve certifikata, preden konfigurirajo VPN za per-app. Če želite več informacij, [glejte Nastavitev navideznega zasebnega omrežja za aplikacijo (VPN) za naprave s sistemom iOS/iPadOS v intunu](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Če želite več informacij o vseh vrstah povezav VPN v intunu, glejte [Ustvarjanje profilov VPN za povezavo s strežniki VPN v intunu](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN za iOS On-Demand se ne sproži, ko je dostopan do konfigurirane domene**

Če želite preskusiti samodejne nastavitve VPN, nastavite te vrednosti:

Želim narediti to: Ovrednotiti **vsak poskus povezave** 

Izberite, ali želite vzpostaviti **povezavo: po potrebi vzpostavite povezavo**

Ko uporabniki dostopajo do teh domen: **ciljno ime** *domene*

Če zgornja konfiguracija ni uspešna, dodajte naslednji element:

Ko ta URL ni dosegljiv, vsili povezavo VPN: **BADURL**