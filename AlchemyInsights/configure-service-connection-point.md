---
title: Konfiguracija točkovne povezave storitve (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037289"
---
# <a name="configure-service-connection-point-scp"></a>Konfiguracija točkovne povezave storitve (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Razlog**: ne morem prebrati predmeta SCP in pridobiti informacije o najemniku v storitvi Azure ad
- **Resolucija**: glejte razdelek [Konfiguracija točke povezave storitve](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Akcijski načrt**

- Preverite, ali je naprava prejela GPO za nadzorovano preverjanje veljavnosti.
- Zagotovite, da je GPO ustvaril registrske ključe.
- Zagotovite, da imate 2 tipki, ustvarjeni z ID-jem imenika in domeno onmicrosoft.

**Konfiguracija nastavitve registra odjemalca za SCP**

Uporabite ta primer, če želite ustvariti predmet pravilnika skupine (GPO), da uvedete nastavitev registra, ki konfigurira vnos SCP v registru naprav.

1. Odprite konzolo za upravljanje pravilnika skupine in ustvarite nov GPO v svoji domeni.
     - Navedite novo ustvarjeno GPO ime (na primer ClientSideSCP)

2. Uredite GPO in poiščite to pot: **Konfiguracija računalnika > nastavitve > nastavitve sistema Windows > register**.

3. Z desno tipko miške kliknite **register** in izberite **nov > element registra**.

4. Na zavihku **splošno** konfigurirajte to:
  
- **Dejanje**: posodobitev
    
- **Panj**: HKEY_LOCAL_MACHINE
    
- **Pot ključa**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Ime vrednosti**: TenantId
    
- **Vrsta vrednosti**: REG_SZ
    
- **Podatki o vrednosti**: GUID ali ID imenika vašega primerka za Azure ad (to vrednost je mogoče najti v **portalu Azure > azure Active Directory > lastnosti > Directory ID**)
 
- Kliknite **V redu**.
 
5. Z desno tipko miške kliknite **register** in izberite **nov > element registra**.

6. Na zavihku **splošno** konfigurirajte to:
  
- **Dejanje**: posodobitev
    
- **Panj**: HKEY_LOCAL_MACHINE
    
- **Pot ključa**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Ime vrednosti**: TenantName
    
- **Vrsta vrednosti**: REG_SZ
    
- **Podatki o vrednosti**: preverjeno ime domene, če uporabljate Združeno okolje, kot je AD FS. Ime preverjene domene ali ime domene onmicrosoft.com (na primer contoso. onmicrosoft). com, če uporabljate upravljano okolje

- Kliknite **V redu**.

7. Zaprite urejevalnik za novo ustvarjeni GPO.

8. Povežite novo ustvarjeni GPO na želeno mesto, ki vsebuje računalnike, ki so povezani z domeno, ki pripadajo vaši nadzorovani populaciji za širitev.

Če želite več informacij, glejte [nadzorovana Validacija hibridnega združevanja v storitvi AZURE ad – AZURE ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) in  [Odpravljanje težav z naprednimi napravami v hibridni storitvi Azure Active Directory | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









