---
title: DLP pravilo za SSN, ne deluje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29933496"
---
Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebino, ki vsebuje **Številko socialnega zavarovanja (SSN)** , pri uporabi vrsto občutljivih podatkov v Office 365? Če je tako, preverite, ali vaša vsebina vsebuje potrebne informacije za DLP politike, kaj išče. 
  
Na primer, za SSN pravilnik, konfiguriran s 85 % stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 številk, ki so lahko v vzorec oblikovano ali Neoblikovano 
    
- **[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije iskati SSNs v štirih različnih vzorcev: 
    
  - Func_ssn najde SSNs s pre-2011 močno oblikovanja, ki so oblikovani s črticami ali prostorov (ddd-dd-dddd ali ddd dd dddd)
    
  - Func_unformatted_ssn najde SSNs s pre-2011 močno oblikovanja, ki so neoblikovano kot devet zaporednih številk (ddddddddd)
    
  - Func_randomized_formatted_ssn najde post-2011 SSNs, ki so oblikovani s črticami ali prostorov (ddd-dd-dddd ali ddd dd dddd)
    
  - Func_randomized_unformatted_ssn najde post-2011 SSNs, ki so neoblikovano kot devet zaporednih številk (ddddddddd)
    
- **[Ček:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, ni ne ček 
    
- **[Opredelitev:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politiko je 85 % prepričan, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov: 
    
  - Vsebina, ki ustreza vzorcu ugotovi, [funkcijo Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) . 
    
  - Ključno besedo iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) je našel. Primeri ključnih besed vključuje: *socialna varnost, socialno varnost #, Soc Sec, SSN* . Na primer, bi ta vzorec sproži za DLP SSN politike: **SSN: 489-36-8350**
    
Več informacij o tem, kaj je potrebno za SSNs treba odkriti za vašo vsebino, glejte naslednji razdelek v tem članku: [Kaj je občutljive vrste informacij iščejo SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

