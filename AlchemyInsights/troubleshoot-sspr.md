---
title: Odpravljanje težav s SSPR-jem
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038974"
---
# <a name="troubleshoot-sspr"></a>Odpravljanje težav s SSPR-jem

**Imam težave s konfiguracijo ponastavitve gesla**

- Če ste skrbnik in iščete navodila za omogočanje samopostrežne ponastavitve gesla, glejte Omogočanje [samopostrežne](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)ponastavitve gesla , če želite konfigurirati ponastavitev gesla za organizacijo. Morda boste želeli pregledati tudi zahteve [za licenciranje.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) V organizaciji morate imeti dodeljeno vsaj eno licenco.
    - **Samo uporabniki v oblaku** – Office 365 inventarna številka (O365) ali Azure AD Basic
    - **Uporabniki v oblaku in/ali** uporabniki na mestu uporabe – Azure AD Premium P1 ali P2, Enterprise Mobility + Security (EMS) ali Secure Productive Enterprise (SPE)
- Če želite dodatna vprašanja o samopostrežni ponastavitvi gesla, si oglejte [pogosta vprašanja.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dobivam sporočilo o napaki**

Preglejte ta članek in poiščite pogoste napake in njihove rešitve: Odpravljanje [težav s samopostrežno ponastavitvijo gesla](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam težavo s pravilnikom za ponastavitev gesla**

- Če se pravilnik za ponastavitev gesla ne obnaša po pričakovanjih ali imate vprašanja o pravilnikih za ponastavitev gesla, preberite ta članek: Pravilniki za gesla in omejitve v [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Pravilniki za ponastavitev gesla ne veljajo za skrbnike. Microsoft za poljubno vlogo skrbnika storitve Azure vsili močan privzeti pravilnik za ponastavitev gesla z dvema prehodoma. Prepričajte se, da preskušate pri uporabniku, ki ni skrbnik. Če želite več informacij o pravilniku za ponastavitev skrbnika, si oglejte ta članek: Razlike v [pravilniku o ponastavitvi skrbnika.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Ne želim, da uporabniki registrirajo dodatne varnostne podatke za ponastavitev gesla**

Podatke (atribute e-pošte in telefona) lahko vnaprej zapolnite za uporabnike, ki uporabljajo API, PowerShell ali Azure AD Povezovalnik. Če želite izvedeti, kako berete:

- [Uvajanje ponastavitve gesla brez zahteve uporabnikov za registracijo](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Katere podatke uporablja ponastavitev gesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Želim, da uporabniki registrirajo svoje dodatne varnostne podatke za ponastavitev gesla**

1. Uporabniki naj registrirajo svoje varnostne podatke za samopostrežno ponastavitev gesla tako, da jih usmerijo [na aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Ko uporabnik (uporabnik ali skrbnik) v polje vnesete podatke, ga usmerite k aka.ms/sspr, da bodo lahko vaši uporabniki ponastavili svoja gesla. [](https://passwordreset.microsoftonline.com/)
1. Če imajo uporabniki še vedno težave, so najverjetneje **neshranjeni** uporabniki s sinhronizirano gesli ali uporabniki z **neshranjeno** gesli. To pomeni, da je verjetno prišlo do težave s storitvijo povratnega pisanja gesla.