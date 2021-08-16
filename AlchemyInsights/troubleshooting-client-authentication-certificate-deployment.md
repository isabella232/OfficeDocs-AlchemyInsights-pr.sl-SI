---
title: Odpravljanje težav s potrdilom za preverjanje pristnosti odjemalca
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020820"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Odpravljanje težav s potrdilom za preverjanje pristnosti odjemalca

Intune NDES/SCEP in profili potrdil odjemalca PKCS/PFX se pogosto uporabljajo skupaj z drugimi vrstami profilov, kot so Wi-Fi, VPN in e-pošta, ki uporabnikom omogočajo preverjanje pristnosti virov podjetja. Ko so te vrste profilov povezane s profilom potrdila odjemalca, so odvisne od uspešne uvedbe tega profila.

Začetna nastavitev infrastrukture in povezana konfiguracija profila odjemalskega potrdila pogosto zahtevata odpravljanje težav. Če želite navodila po korakih za uspešno nastavitev povezovalnika NDES in navodila za odpravljanje težav z osamitvijo težav z uvedbo potrdila, glejte: 

- [Konfiguracija infrastrukture za podporo SCEP-a s intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled odpravljanja težav s profili potrdil SCEP Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

S skripti Powershell, na katere se sklicujete, lahko preverite konfiguracijo. Če želite več informacij, glejte Skripti za [preverjanje povezovalnika potrdila za Intune.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Druge pogoste težave**

**Ko poskusim namestiti povezovalnik potrdila za Intune v povezovalnik NDES, se prikaže sporočilo »Gesla v zahtevi za potrdilo ni mogoče preveriti. Morda je bil že uporabljen. Pridobite novo geslo za pošiljanje s to zahtevo.«**  

To sporočilo pomeni, da morate kot skrbnik zagnati namestitev povezovalnika potrdila.

V nekaterih okoljih morajo strežniki, v katerih se izvaja potrdilo za Intune, za vzpostavitev povezave s storitvijo Intune uporabiti strežnik proxy, zato mora povezovalnik potrdila uporabiti proxy. V nekaterih primerih povezovalnik NDES prezre konfigurirane nastavitve proxyja in morda je treba konfigurirati nastavitve proxyja med izvajanjem v varnostnem kontekstu sistema LocalSystem. 
 
Rešitev je, da zaženete Internet Explorer kot SISTEM in konfigurirate proxy v Internet Explorerju. Po vnovičnem zagonu storitve Intune Connector se povezovalnik NDES poveže s storitvijo Intune.

**Uporabniške naprave ne prejemajo več potrdil SCEP iz storitve NDES.**

Možno je, da je potrdilo za preverjanje pristnosti odjemalca, izdano za strežnik NDES in določeno med namestitvijo povezovalnika NDES, poteklo ali pa manjka. Če želite odpraviti to težavo: 
 
1. Odstranite priključek NDES.  
2. Uporabite te podrobnosti, če želite zahtevati novo preverjanje pristnosti odjemalca ali potrdilo za preverjanje pristnosti strežnika: 
 
    - Ime zadeve: CN=external fqdn  
    - Nadomestno ime zadeve (oboje je zahtevano): DNS=zunanji fqdn, DNS=internal fqdn 
 
3. Znova namestite povezovalnik NDES z novim potrdilom.