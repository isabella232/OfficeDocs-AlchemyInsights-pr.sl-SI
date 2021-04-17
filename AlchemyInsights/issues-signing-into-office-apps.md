---
title: Težave pri vpisu v aplikacije Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833031"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Sporočilo o odpravljanju težav v aplikacijah Microsoft 365 »Modul zaupanja vredne platforme vašega računalnika ne deluje pravilno«

Če želite to napako odpraviti, poskusite to:

- Namestite najnovejše posodobitve za [Windows in](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Počistite poverilnice za Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Poskusite postopek [obnovitve uporabnika, da](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) odpravite napake modula zaupanja vrednih platform (TPM).
- Nastavite EnableADAL = 0 tako, da sledite tem korakom:  
    1. Z desno tipko miške kliknite gumb Start sistema Windows, **izberite Zaženi**, vnesite **regedit** in nato izberite V **redu**.
    2. Če **želite** urejevalniku registra dovoliti spreminjanje naprave, izberite Da.
    3. V urejevalniku registra dodajte vrednost DWORD za **EnableADAL** z nastavitvijo **0** v razdelku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Če želite več informacij, glejte Težave pri vpisu s povezavo po posodobitvi na [gradovi Office 2016, graden 16.0.7967 v sistemu Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)