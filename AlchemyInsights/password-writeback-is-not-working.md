---
title: Password Writeback ne deluje
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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324939"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback ne deluje

**Imam težave s konfiguracijo povratnega pisanja gesla**

- Funkcija pisanja gesla je vrhunska funkcija.
- Prepričajte se, da razumete zahteve za licenciranje:
  - V organizaciji morate imeti dodeljeno vsaj eno licenco
  - **Samo uporabniki v oblaku** – Office 365 (O365) plačljiva inventarna številka ali Azure AD Basic
  - **Uporabniki v oblaku in/ali** uporabniki na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure Productive Enterprise (SPE)
    - Če želite izvedeti več o zahtevah licenciranja, glejte [Zahteve licenciranja za](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) samopostrežno ponastavitev gesla za Azure AD
- Imate vsaj en skrbniški račun in en preskus uporabniškega računa z eno od ustreznih licenc.
- Če želite, da deluje povratne Povezovalnik z geslom, morate povezati aplikacijo Azure AD in emulator primarnega krmilnika domene. Imenik Azure AD lahko konfigurirate tako Povezovalnik da uporablja primarni  kontrolnik domene, tako da z desno tipko miške kliknete lastnosti povezovalnika za sinhronizacijo imenika Active Directory, nato pa izberete konfiguriraj particije **imenika.** Tam poiščite razdelek z nastavitvami povezave **za krmilnik** domene in potrdite polje z naslovom uporabi le **priljubljene kontrolnike domene**.
    **Opomba:Če** prednostni DC ni emulator PDC, se bo imenik Azure AD Povezovalnik še vedno stikl s PDC-jem in geslom za pisanje.
- Ponastavitev gesla je bila konfigurirana in omogočena v vašem najemniku. Če želite več informacij, glejte [Omogočanje uporabnikom, da ponastavijo svoja gesla za Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Prepričajte se, da je skrbniški račun, ki se uporablja za omogočanje povratnega pisanja gesla, skrbniški račun v oblaku (ustvarjen v imeniku Azure AD, ki ni ad na mestu uporabe)
- Uporabljate eno ali več gozdno uvajanje AD na mestu uporabe, ki se izvaja Windows Server 2008 R2, Windows Server 2012 ali Windows Server 2012 R2 z nameščenimi najnovejšimi servisnimi paketi
- Imate nameščeno orodje za Povezovalnik Azure AD in pripravite okolje AD za sinhronizacijo z oblakom. Preden preskusite pisanje gesla, morate najprej dokončati poln uvoz in popolno sinhronizacijo iz imenika AD in imenika Azure AD v imeniku Azure AD Povezovalnik.
- Če želite izvedeti več, si oglejte, kako lahko v [imeniku Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations) popolnoma sinhronizirate in v celoti Povezovalnik

**Imam težave z povezljivostjo povratnega pisanja gesel**

1. Prenesite in omogočite najnovejšo različico [imenika Azure AD Povezovalnik](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija požarnega zidu: orodje Azure AD Povezovalnik (1.1.443 in več) potrebuje odhodni **dostop HTTPS** za:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Omogočanje, da se povezave nedejavnosti ohranijo vsaj 2–3 minute

**Še vedno imam težave s pisanjem gesla**

- Če imate še vedno težave, poskusite onemogočiti in znova omogočiti storitev pisanja gesla v orodju Azure AD Povezovalnik 10
- Če želite izvedeti več, si [oglejte, kako onemogočite in znova omogočite pisanje gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
