---
title: Težave pri vpisu v programe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695195"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravljanje aplikacije Microsoft 365 apps» modul zaupanja vredne platforme računalnika ni pravilno delujoč «

Če želite to napako odpraviti, poskusite to:

- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Počistite Officeove poverilnice](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Preskusite [postopek za obnovitev uporabnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , da odpravite napake modula zaupanja TPM.
- Nastavite EnableADAL = 0 s temi koraki:  
    1. Z desno tipko miške kliknite gumb Start sistema Windows, izberite **Zaženi**, vnesite **regedit**in nato izberite **v redu**.
    2. Izberite **da** , da omogočite urejevalnik registra, da spremenite vašo napravo.
    3. V urejevalniku registra dodajte vrednost DWORD **EnableADAL** z nastavitvami **0** v razdelku HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi na Office 2016 Build 16.0.7967 v sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).