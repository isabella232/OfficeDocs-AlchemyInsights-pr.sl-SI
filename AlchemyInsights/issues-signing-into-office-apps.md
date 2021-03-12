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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709122"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravljanje aplikacije Microsoft 365 apps» modul zaupanja vredne platforme računalnika ni pravilno delujoč «

Če želite to napako odpraviti, poskusite to:

- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Preskusite [postopek za obnovitev uporabnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , da odpravite napake modula zaupanja TPM.
- Nastavite EnableADAL = 0 s temi koraki:  
    1. Z desno tipko miške kliknite gumb Start sistema Windows, izberite **Zaženi**, vnesite **regedit** in nato izberite **v redu**.
    2. Izberite **da** , da omogočite urejevalnik registra, da spremenite vašo napravo.
    3. V urejevalniku registra dodajte vrednost DWORD **EnableADAL** z nastavitvami **0** v razdelku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi na Office 2016 Build 16.0.7967 v sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).