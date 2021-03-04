---
title: Odpravljanje težav z SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430214"
---
# <a name="troubleshoot-sspr"></a>Odpravljanje težav z SSPR

**Imam težave pri konfiguraciji ponastavitev gesla**

- Če ste skrbnik in si želite ogledati, kako omogočite samopostrežno ponastavitev gesla, glejte [Vadnica omogoči SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), da konfigurirate ponastavitev gesla za vašo organizacijo. Morda boste želeli pregledati tudi zahteve za [licenciranje](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). V vaši organizaciji morate dodeliti vsaj eno licenco.
    - **Samo uporabniki v oblaku** – vsak Office 365 (O365) plačan sku ali Azure ad Basic
    - **Uporabniki v oblaku in/ali na mestu uporabe** – Azure ad Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure produktivno podjetje (SPE)
- Če želite dodatna vprašanja o samopostrežnem ponastavitvi z geslom, si oglejte [naša vprašanja](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Dobivam sporočilo o napaki**

Oglejte si ta članek, če želite poiskati pogoste napake in njihove rešitve: [Odpravljanje težav z ponastavitvijo samopostrežnega gesla](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam težave s pravilnikom za ponastavitev gesla**

- Če pravilnik za ponastavitev gesla ni v skladu s pričakovanji, ali če imate vprašanja o pravilnikih za ponastavitev gesla, si oglejte ta članek: [Pravilniki o geslih in omejitve v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Pravilniki za ponastavitev gesla se ne nanašajo na skrbnike. Microsoft uveljavi močne privzete pravilnike za ponastavitev gesla za vsako vlogo v storitvi Azure skrbnika. Prepričajte se, da preizkušate uporabnika, ki ni skrbnik. Če želite več informacij o pravilniku za ponastavitev skrbnika, si oglejte ta članek: [Ponastavi razlike pravilnika za skrbnike](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Ne želim, da moji uporabniki registrirajo dodatne varnostne informacije za ponastavitev gesla**

Za uporabnike lahko vnaprej zapolnite podatke (e-poštne in telefonske atribute), ki uporabljajo API, PowerShell ali Azure AD Connect. Če želite izvedeti, kako brati:

- [Uvajanje ponastavitev gesla brez zahteve za registracijo uporabnikov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Katere podatke uporablja ponastavitev gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Želim, da moji uporabniki registrirajo svoje dodatne varnostne informacije za ponastavitev gesla**

1. Naj vaši uporabniki registrirajo svoje varnostne informacije za samoponastavitev gesla, tako da jih usmerjajo v [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Ko so podatki poseljeni za uporabnika (uporabnik ali skrbnik), usmerite uporabnika v [aka.MS/sspr](https://passwordreset.microsoftonline.com/) , da bodo uporabniki lahko ponastavili svoja gesla.
1. Če uporabniki še vedno doživljajo težave, so uporabniki, ki so najverjetneje **združevali** ali **razpršili geslo, sinhronizirani** . To pomeni, da je prišlo do težave z geslom storitve Nepotrjenim.