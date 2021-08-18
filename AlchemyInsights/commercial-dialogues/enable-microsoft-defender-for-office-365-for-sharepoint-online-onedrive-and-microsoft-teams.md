---
title: Omogočanje Sef prilog za SharePoint Online, OneDrive in Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332395"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogočanje Sef prilog za SharePoint Online, OneDrive in Microsoft Teams

1. S poverilnicami globalnega skrbnika ali skrbnika za varnost odprite portal Microsoft 365 Defender na spletnem mestu , nato pa se v razdelku Pravilniki & pravilniki za pravilnike o grožnjah za Sef priloge v razdelku <https://security.microsoft.com>  \>  \>  »Pravilniki« 

   Če se želite neposredno po **Sef Priloge,** uporabite <https://security.microsoft.com/safeattachmentv2> .

2. Na **strani Sef Priloge** kliknite **Globalne nastavitve.**
3. V prikazanem podoknu izberite Vklopi Microsoft Defender za Office 365 za **SharePoint, OneDrive** in Microsoft Teams , nato pa izberite **Shrani**.

    **Namig:** Če želite izboljšati zaščito prilog za Sef, naredite SharePoint, OneDrive in Microsoft Teams:
    - Če želite uporabnikom preprečiti prenos zlonamernih datotek, uporabite vrednost `$true` parametra *DisallowInfectedFileDownload* v ukazu »cmdlet« **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** v SharePoint Online PowerShell. Če želite več informacij, glejte Uporaba SharePoint Online PowerShell za preprečevanje uporabnikom [prenos zlonamernih datotek.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Ustvarjanje pravilnika opozoril za zaznane datoteke](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Če želite več informacij, [Sef Priloge za Office 365 za SharePoint, OneDrive in Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
