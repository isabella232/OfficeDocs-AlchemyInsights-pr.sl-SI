---
title: Odpravljanje težav pri uvajanju potrdila za preverjanje pristnosti odjemalca
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555809"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Odpravljanje težav pri uvajanju potrdila za preverjanje pristnosti odjemalca

Profili certifikatov NDES/SCEP in PKCS/PFX client se običajno uporabljajo v povezavi z drugimi vrstami profilov, kot so Wifi, VPN in e-pošta, ki uporabnikom omogočajo preverjanje pristnosti s poslovnimi viri. Če so te vrste profilov povezane s profilom potrdila odjemalca, so odvisne od uspešne uvedbe tega profila.

Začetna nastavitev infrastrukture in povezana konfiguracija profila odjemalskega potrdila pogosto zahtevata odpravljanje težav. Navodila za uspešno namestitev konektorja NDES in navodila za odpravljanje težav za izolacijo težav pri uvajanju certifikatov so na voljo v navodilih za odpravljanje težav, glejte: 

- [Konfiguracija infrastrukture za podporo SCEP z Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled za odpravljanje težav s certifikatnimi profili SCEP z MicrosoftOm Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

S skripti powershell, na katere se sklicujete, lahko preverite konfiguracijo. Če želite več informacij, [glejte Skripti za preverjanje potrdila intune .](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Druga pogosta vprašanja**

**Ko poskušam namestiti konektor potrdila Intune na strežniku konektorja NDES, se prikaže sporočilo »Gesla v zahtevi za potrdilo ni mogoče preveriti. Morda je že bil uporabljen. Pridobite novo geslo za pošiljanje s to zahtevo."**  

To sporočilo pomeni, da morate namestitev certifikatnega konektorja zagnati kot skrbnika.

V nekaterih okoljih morajo strežniki, v katerih se izvaja potrdilo Intune, za povezavo z intunom uporabiti proxy strežnik, zato mora certifikatni konektor uporabljati proxy. V nekaterih okoliščinah NDES Connector prezre konfigurirane nastavitve strežnika proxy in morda bo treba konfigurirati nastavitve strežnika proxy med izvajanjem v varnostnem kontekstu lokalnega sistema. 
 
Rešitev je, da zaženete Internet Explorer kot SYSTEM in konfigurirate proxy v IE. Po vnovičnem zagonu storitve intune connector se konektor NDES poveže z intunom.

**Uporabniške naprave ne prejemajo več certifikatov SCEP od NDES-a.**

Možno je, da je potrdilo za preverjanje pristnosti odjemalca, izdano strežniku NDES in je določeno med namestitvijo konektorja NDES, poteklo ali manjka. Če želite odpraviti: 
 
1. Odstranite konektor NDES.  
2. Te podrobnosti uporabite, če želite zahtevati novo preverjanje pristnosti odjemalca ali potrdilo za preverjanje pristnosti strežnika: 
 
    - Ime zadeve: CN=zunanji fqdn  
    - Nadomestno ime zadeve (oba sta potrebna): DNS=zunanji fqdn, DNS=notranji fqdn 
 
3. Znova namestite konektor NDES z novim potrdilom.