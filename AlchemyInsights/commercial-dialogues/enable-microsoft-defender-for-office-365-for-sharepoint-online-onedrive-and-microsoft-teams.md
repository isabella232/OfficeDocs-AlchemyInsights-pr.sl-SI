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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894479"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogočanje Sef prilog za SharePoint Online, OneDrive in Microsoft Teams

1. S poverilnicami globalnega skrbnika ali skrbnika za varnost odprite portal Microsoft 365 Defender v razdelku , nato pa se v razdelku Pravilniki & pravilniki za pravilnike o grožnjah za Sef Priloge v razdelku <https://security.microsoft.com>  \>  \>  Pravilniki. 

   Če se želite neposredno po **Sef Priloge,** uporabite <https://security.microsoft.com/safeattachmentv2> .

2. Na **strani Sef Priloge** kliknite **Globalne nastavitve.**
3. V prikazanem flyoutu izberite **Vklopi Microsoft Defender za Office 365 za SharePoint, OneDrive** in Microsoft Teams , nato pa izberite **Shrani**.

    > [!TIP]
    >
    > Če želite izboljšati zaščito prilog za Sef za SharePoint, OneDrive in Microsoft Teams:
    >
    > - Če želite uporabnikom preprečiti prenos zlonamernih datotek, uporabite vrednost `$true` parametra *DisallowInfectedFileDownload* v ukazu »cmdlet« **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** v SharePoint Online PowerShell. Če želite več [informacij, glejte Uporaba SharePoint Online PowerShell za preprečevanje uporabnikom prenos zlonamernih datotek.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Ustvarjanje pravilnika opozoril za zaznane datoteke](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Če želite več informacij, [glejte Sef Priloge za Office 365 za SharePoint, OneDrive in Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
