---
title: Težave pri vpisu v Microsoft 365 apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579881"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravljanje Microsoftovih 365 aplikacij» modul zaupanja vrednih platform računalnika ne deluje pravilno «

Če želite to napako odpraviti, poskusite to:

- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Počistite Officeove poverilnice](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.<br/>
    **Opomba:** Registrske poti za Office 2016 so se spremenile v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Preizkusite [postopek za obnovitev uporabnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , da odpravite napake modula zaupanja vrednih platform (TPM).
- Nastavite EnableADAL = 0 z naslednjimi koraki:  
    1. Z desno tipko miške kliknite gumb Start sistema Windows, izberite **Zaženi**, vnesite **regedit**in izberite **v redu**.
    2. Izberite **da** , če želite urejevalniku registra omogočiti spreminjanje naprave.
    3. V urejevalniku registra dodajte vrednost DWORD **Enableadal** z nastavitvijo **0** pod HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.

Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi v Office 2016 graditi 16.0.7967 v operacijskem sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).