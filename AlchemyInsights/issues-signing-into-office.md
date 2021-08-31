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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744662"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Težave pri vpisu v Programi Microsoft 365

Opomba: Če uporabljate starejšo različico programa Windows (npr. Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), uporabite preprost popravek, da za privzeto omogočite TLS 1.2. Če želite več informacij, glejte Posodobitev, da omogočite [TLS 1.1 in TLS 1.2 kot](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)privzete varne protokole v winhttp v brskalniku Windows.

Če želite odpraviti težave s Programi Microsoft 365, poskusite izvesti te možnosti zadevni napravi:  

- Če Windows več Priporočila [o odpravljanju pogostih](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) težav z vpisom
- Za Mac glejte [Ne morem se vpisati v aplikacijo Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Namig** na računalnikih s sistemom Windows lahko diagnosticirate in samodejno odpravite več pogostih težav pri vpisu v Office. Prenesite in zaženite orodje **[Pomočnik za podporo in obnovitev](https://aka.ms/SaRA-OfficeSignInScenario)** za uporabo avtomatiziranega orodja.

**Opomba:** Onemogočanje sodobnega preverjanja pristnosti (ADAL) ali storitve Microsoft Web Account Management (WAM) za odpravljanje težav z vpisom ali aktiviranjem **ni priporočljivo.** Če pri vzpostavljanju povezave s programom Microsoft 365 Office 2013 pride do [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) napak, zagotovite, da omogočite sodobno preverjanje pristnosti za Office odjemalca.

Za določena dejanja odpravljanja težav glejte:

[Težave pri vpisu po posodobitvi na Office 2016, graden 16.0.7967 v Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Ne morete se vpisati v račun organizacije, kot je Office 365, Azure ali Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Odpravljanje težav z aplikacijami, ki niso brskalniki, ki se ne morejo vpisati v Office 365, Azure ali Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Večkrat pozvan k vnosu poverilnic v Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)