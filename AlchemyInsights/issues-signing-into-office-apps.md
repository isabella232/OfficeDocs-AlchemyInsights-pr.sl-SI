---
title: Težave pri vpisu v Microsoft 365 aplikacije
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986907"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Če popravite Microsoft 365 sporočilo »Modul zaupanja vredne platforme vašega računalnika ne deluje pravilno«

Če želite to napako odpraviti, poskusite to:

- Namestite najnovejše posodobitve [za](https://support.microsoft.com/help/4027667/windows-10-update) Windows [in Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Počistite Office poverilnic](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) s Windows upravitelja poverilnic.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Poskusite postopek [obnovitve uporabnika, da](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) odpravite napake modula zaupanja vrednih platform (TPM).
- Nastavite EnableADAL = 0 tako, da sledite tem korakom:  
    1. Z desno tipko miške kliknite Windows Start, izberite **Zaženi**, vnesite **regedit** in nato izberite V **redu**.
    2. Če **želite** urejevalniku registra dovoliti spreminjanje naprave, izberite Da.
    3. V urejevalniku registra dodajte vrednost DWORD za **EnableADAL** z nastavitvijo **0** v razdelku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Če želite več informacij, glejte Težave pri vpisu s povezavo po posodobitvi na grad Office [2016 16.0.7967 v Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)