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
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999760"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback ne deluje

**Imam težave s konfiguracijo povratnega pisanja gesla**

- Funkcija pisanja gesla je vrhunska funkcija.
- Prepričajte se, da razumete zahteve za licenciranje:
  - V organizaciji morate imeti dodeljeno vsaj eno licenco
  - **Samo uporabniki v oblaku** – Office 365 inventarna številka (O365) ali Azure AD Basic
  - **Uporabniki v oblaku in/ali** uporabniki na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure Productive Enterprise (SPE)
    - Če želite izvedeti več o zahtevah licenciranja, glejte [Zahteve licenciranja za](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) samopostrežno ponastavitev gesla za Azure AD
- Imate vsaj en skrbniški račun in en preskus uporabniškega računa z eno od ustreznih licenc.
- Če želite, da deluje povratne Povezovalnik z geslom, morate povezati aplikacijo Azure AD in emulator primarnega krmilnika domene. Azure AD Povezovalnik za uporabo primarnega krmilnika domene tako,  da z desno tipko miške kliknete lastnosti povezovalnika za sinhronizacijo imenika Active Directory, nato pa izberete konfiguriraj particije **imenika.** Tam poiščite razdelek z nastavitvami povezave **za krmilnik** domene in potrdite polje z naslovom uporabi le **priljubljene kontrolnike domene**.
  > [!NOTE]
  > Če prednostni DC ni emulator PDC, se bo imenik Azure AD Povezovalnik še vedno stik s pdc-jem in vam vrnil geslo.
- Ponastavitev gesla je bila konfigurirana in omogočena v vašem najemniku. Če želite več informacij, glejte [Omogočanje uporabnikom, da ponastavijo svoja gesla za Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Prepričajte se, da je skrbniški račun, ki se uporablja za omogočanje povratnega pisanja gesla, skrbniški račun v oblaku (ustvarjen v imeniku Azure AD, ki ni ad na mestu uporabe)
- V strežniku Windows Server 2008 R2, Windows Server 2012 ali Windows Server 2012 R2 imate eno ali več gozdno uvajanje z nameščenimi najnovejšimi servisnimi paketi
- Nameščeno imate orodje Azure AD Povezovalnik in pripravite okolje AD za sinhronizacijo z oblakom. Preden preskusite pisanje gesla, morate najprej dokončati poln uvoz in popolno sinhronizacijo iz imenika AD in imenika Azure AD v imeniku Azure AD Povezovalnik.
- Če želite izvedeti več, preberite, kako lahko v imeniku Azure AD v celoti sinhronizirate [in Povezovalnik](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Imam težave s povezljivostjo povratnega pisanja gesel**

1. Prenesite in omogočite najnovejšo različico [imenika Azure AD Povezovalnik](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija požarnega zidu: orodje Azure AD Povezovalnik (1.1.443 in višje) potrebuje **odhodni dostop HTTPS** za:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Omogočanje, da se povezave nedejavnosti ohranijo vsaj 2–3 minute

**Še vedno imam težave s pisanjem gesla**

- Če imate še vedno težave, poskusite onemogočiti in znova omogočiti storitev pisanja gesla v orodju Azure AD Povezovalnik 10
- Če želite izvedeti več, si [oglejte, kako onemogočite in znova omogočite pisanje gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
