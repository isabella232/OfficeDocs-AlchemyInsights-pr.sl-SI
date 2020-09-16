---
title: Odpravljanje težav z uvajanjem potrdila o pristnosti odjemalca
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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659002"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Odpravljanje težav z uvajanjem potrdila o pristnosti odjemalca

InTune NDES/SCEP in PKCS/PFX profili potrdil odjemalca se običajno uporabljajo v povezavi z drugimi vrstami profilov, kot so WiFi, VPN in e-pošta, da uporabnikom omogočijo preverjanje pristnosti za vire podjetja. Ko so te vrste profilov povezane s profilom potrdila odjemalca, so odvisne od uspešne uvedbe tega profila.

Začetna nastavitev infrastrukture in povezana konfiguracija profila odjemalčevega potrdila pogosto zahtevata odpravljanje težav. Če želite navodila po korakih za uspešno nastavitev povezovalnika NDES in navodila za odpravljanje težav pri izoliranju težav s uvajanjem potrdila, glejte: 

- [Konfiguracija infrastrukture za podporo SCEP z InTune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled za odpravljanje težav SCEP profilov potrdil z Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Uporabite referenčne skripte PowerShell za pomoč pri preverjanju konfiguracije. Če želite več informacij, glejte Iskanje [skriptov za preverjanje priključka potrdila](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Druge pogoste težave**

**Ko poskusim namestiti povezovalnik» InTune «v strežniku NDES Connector, dobim sporočilo, da» gesla v zahtevi za potrdilo ni mogoče preveriti. Morda je bil že uporabljen. Pridobite novo geslo, ki ga želite poslati s to zahtevo. «**  

To sporočilo pomeni, da morate zagnati namestitev povezovalnika potrdila kot skrbnik.

V nekaterih okoljih morajo strežniki, v katerih se izvaja potrdilo InTune, uporabljati proxy strežnik, s katerim lahko vzpostavite povezavo s funkcijo InTune, zato mora povezovalnik potrdil uporabiti proxy. V nekaterih primerih povezovalnik NDES prezre konfigurirane nastavitve proxyja in bo morda treba konfigurirati nastavitve strežnika proxy, medtem ko se izvaja v varnostnem kontekstu LocalSystem. 
 
Rešitev je, da zaženete Internet Explorer kot sistem in konfigurirate proxy v IE. Po vnovičnem zagonu storitve priključka za InTune se NDES povezovalnik poveže z InTune.

**Uporabniške naprave ne prejemajo več SCEP potrdil iz NDES.**

Možno je, da je potrdilo o pristnosti odjemalca, izdano v strežnik NDES, in določeno med namestitvijo povezovalnika NDES, poteklo ali manjka. Če želite razrešiti: 
 
1. Odstranite povezovalnik NDES.  
2. S temi podrobnostmi lahko zahtevate novo preverjanje pristnosti odjemalca ali potrdilo za preverjanje pristnosti strežnika: 
 
    - Ime zadeve: CN = zunanji FQDN  
    - Ime nadomestnega predmeta (oba sta obvezna): DNS = zunanji FQDN, DNS = Internal FQDN 
 
3. Znova namestite povezovalnik NDES z novim potrdilom.