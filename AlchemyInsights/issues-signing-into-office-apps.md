---
title: Vprašanja, ki se vpisujete Office aplikacije
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938344"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Določitev urad apps "modula zaupanja TPM računalnika ne deluje pravilno" sporočilo

Če želite odpraviti to napako, poskusite naslednje:

- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Jasno urad poverilnic](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.<br/>
    **Opomba:** Registrske poti za Office 2016 spremenili v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Začeti [postopek izterjave uporabnik](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) popraviti napake Modul TPM (Trusted Platform).
- Nastaviti v EnableADAL = 0, po naslednjih korakih:  
    1. Z desno tipko miške na gumb Start, izberite **Zaženi**, vnesite **regedit**in izberite **OK**.
    2. Izberite **ja** omogočiti urejevalnik registra, da spremenite napravo.
    3. V registracija urednik, dodajte vrednost DWORD **EnableADAL** s nastavitev **0** pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Če želite več informacij, glejte [te¾ave pri povezovanju v vpisno po posodobitvi za Office 2016 zidava 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).