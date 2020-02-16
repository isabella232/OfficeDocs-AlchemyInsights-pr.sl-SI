---
title: Popravljanje Officeovih aplikacij vaš račun je v slabem stanju sporočilo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969803"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Popravljanje Officeovih aplikacij» vaš račun je v slabem stanju «

Če želite odpraviti to napako, poskusite naslednje možnosti v prizadetem računalniku:

- Odprite Officeovo aplikacijo, izberite račun **datotečnega** > **računa** > **iz vseh računov**. Znova se vpišite z uporabniškim računom z veljavno licenco. Za podrobnejše informacije glejte [računi v Officeu](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.<br>
  **Opomba:** Registrske poti za Office 2016 so se spremenile v 16,0. Na primer \Software\Microsoft\Office\16.0\Common\Identity\
- V prizadetem računalniku nastavite EnableADAL = 0 z naslednjimi koraki:  
     1. Z desno tipko miške kliknite gumb Windows in izberite **Zaženi**. V polje **Odpri** vnesite **regedit**in nato izberite **v redu**.
     2. Izberite **da** , ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.
    3. V urejevalniku registra dodajte vrednost DWORD EnableADAL z nastavitvijo 0 pod HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Če pride do napake med povezovanjem z Officeom 365 z Officeom 2013, [omogočite sodobno preverjanje pristnosti](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) za odjemalca Office.

Če želite več informacij, glejte [Odpravljanje težav z aplikacijami brez brskalnika, ki se ne morejo prijaviti v Office 365, Azure ali InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

