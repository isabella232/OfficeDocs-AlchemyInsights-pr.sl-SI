---
title: Omogočanje Office 365 ATP za SharePoint, OneDrive in Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964649"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogočite Microsoft Defender za Office 365 za SharePoint Online, OneDrive in Microsoft Teams

1. Pojdite v https://protection.office.com in se vpišite.
2. Izberite **Pravilnik za upravljanje**  >  **groženj** Sef  >  **priloge.**
3. Izberite **Vklopi Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams** in nato kliknite **Shrani.**
4. (Priporočeno) Kot globalni skrbnik ali skrbnik storitve SharePoint Online zaženite ukaz »cmdlet« [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload,** nastavljenim na *true.*
5. (Priporočeno) [Nastavite opozorila](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za zaznane datoteke.

> [!NOTE]
> Microsoft Defender for Office 365 ne bo optično preglejl vseh datotek v storitvi SharePoint Online, OneDrive ali Microsoft Teams. Datoteke so pregledane asinhrono, s postopkom, ki uporablja dogodke skupne rabe in dejavnosti gostov, skupaj s pametnimi heuristično in signali groženj za identifikacijo zlonamernih datotek. Glejte [Microsoft Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)