---
title: Geslo Nepotrjenim ne deluje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243523"
---
# <a name="password-writeback-is-not-working"></a>Geslo Nepotrjenim ne deluje

**Imam težave pri konfiguraciji gesla nepotrjenim**

- Geslo nepotrjenim je funkcija Premium.
- Prepričajte se, da razumete zahteve za licenciranje:
  - Imeti morate vsaj eno licenco, dodeljeno v organizaciji.
  - **Samo uporabniki v oblaku** – vsak Office 365 (O365) plačan sku ali Azure ad Basic
  - **Uporabniki v oblaku in/ali na mestu uporabe** – Azure ad Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)
    - Če želite izvedeti več o zahtevah za licenciranje, glejte [zahteve za licenciranje za samopostrežno ponastavitev gesla za AZURE ad.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Imate vsaj en skrbniški račun in en preskusni uporabniški račun z eno od ustreznih licenc.
- Če želite delati z geslom za nepotrjenim, morate povezati Azure AD, da se povežete z Emulatorjem primarnega krmilnika domene. Če želite uporabiti primarni krmilnik domene, lahko konfigurirate povezavo storitve Azure AD, tako da z desno tipko miške kliknete **lastnosti** povezovalnika imenika Active Directory in nato izberete **Konfiguracija particij imenikov**. V razdelku poiščite razdelek **Nastavitve povezave krmilnika domene** in potrdite polje z naslovom **uporabi le želene krmilnike domene**.
  > [!NOTE]
  > Če želeni DC ni Emulator PDC, bo Azure AD Connect še vedno vzpostavil dostop do PDC za geslo nepotrjenim.
- Ponastavitev gesla je bilo konfigurirano in omogočeno v najemniku. Če želite več informacij, glejte [Omogočanje uporabnikom, da ponastavijo gesla za AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Prepričajte se, da je skrbniški račun uporabljen za omogočanje gesla Nepotrjenim je skrbniški račun za oblak (ustvarjen v storitvi Azure AD not AD na mestu uporabe)
- Imate eno ali več-gozdno uvajanje na mestu uporabe s sistemom Windows Server 2008 R2, Windows Server 2012 ali Windows Server 2012 R2 z nameščenimi najnovejšimi servisnimi paketi
- Imate nameščeno orodje za povezovanje v storitvi Azure AD in ste pripravili svoje OGLAŠEVALsko okolje za sinhronizacijo z oblakom. Preden preskusite geslo za nepotrjenim, se prepričajte, da ste najprej dokončali popolno uvoz in popolno sinhronizacijo iz oglasov AD in Azure AD v storitvi Azure AD Connect.
- Če želite izvedeti več, glejte Kako narediti [popolno sinhronizacijo in poln uvoz v storitvi AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Imam težave s povezljivostjo z geslom nepotrjenim**

1. Prenesite in omogočite najnovejšo različico storitve [AZURE ad Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija požarnega zidu: orodje za povezovanje v storitvi Azure AD (1.1.443 in zgoraj) bo moralo dostopati do programa **https** :
    - passwordreset.microsoftonline.com
    - servicebus. Windows. Networks
3. Dovoli nedejavne povezave, da trajajo vsaj 2-3 minut

**Še vedno imam težave z geslom nepotrjenim**

- Če imate še vedno težave, poskusite onemogočiti in znova omogočiti storitev nepotrjenim gesel v orodju za povezovanje v storitvi Azure AD.
- Če želite izvedeti več, glejte kako [onemogočiti in znova omogočiti nepotrjenim gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
