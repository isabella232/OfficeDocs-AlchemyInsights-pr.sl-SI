---
title: DLP pravilo za številko kreditne kartice, ne deluje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919096"
---
Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebino, ki vsebuje **Številko kreditne kartice** , pri uporabi vrsto DLP občutljive informacije v O365? Če je tako, se prepričajte, vaše vsebine vsebuje potrebne informacije za sprožitev z DLP politike, ko je ovrednotena. Na primer, za **politike kreditne kartice** konfiguriran z 85 % stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 števk, kar lahko oblikovano ali neoblikovano (dddddddddddddddd) in mora prestati preskus Luhn. 
    
- **[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zelo kompleksna in močna vzorec, ki zazna kartice iz vseh večjih blagovnih znamk po vsem svetu, vključno z Visa, Mastercard, odkriti kartico, JCB, American Express, darilne kartice in kartice diner. 
    
- **[Ček:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn ček 
    
- **[Opredelitev:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politiko je 85 % prepričan, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov: 
    
  - Vsebina, ki ustreza vzorcu ugotovi, funkcijo Func_credit_card.
    
  - Je izpolnjen eden od naslednjih: 
    
  - Ključno besedo iz Keyword_cc_verification je našel.
    
  - Ključno besedo iz Keyword_cc_name je našel
    
  - Funkcijo Func_expiration_date ugotovi datum v pravi datumski obliki.
    
  - Ček prehaja
    
    Na primer, ta vzorec bi sproži za DLP kreditne kartice številko politike:
    
  - Vizum: 4485 3647 7352 3952 
    
  - Poteče: 2/2009
    
Več informacij o tem, kaj je potrebno za **Številko kreditne kartice** za vašo vsebino, je mogoče odkriti, glejte naslednji razdelek v tem članku: [Kaj je občutljive vrste informacij iščejo kreditne kartice #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

