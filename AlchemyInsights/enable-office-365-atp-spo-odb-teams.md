---
title: Omogočanje sistema Office 365 ATP za SharePoint, OneDrive in Microsoft Teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709923"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogočanje napredne zaščite pred grožnjami za Office 365 za SharePoint online, OneDrive in Microsoft Teams

1. Pojdite na https://protection.office.com in se vpišite.
2. Izberite **Threat management**  >  **Policy**  >  **varna Priloga**pravilnika za upravljanje groženj.
3. Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams**in nato kliknite **Shrani**.
4. Priporočeno Kot globalni skrbnik ali skrbnik SharePoint Onlinea zaženite ukaz» cmdlet « [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** , nastavljenim na *True*.
5. Priporočeno [Nastavite opozorila](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za zaznane datoteke.

> [!NOTE]
> ATP bo pregledal vsako posamezno datoteko v storitvi SharePoint online, OneDrive ali Microsoft teams. Datoteke so asinhrono skenirane, in sicer s postopkom, ki uporablja dogodke skupne rabe in gostujoče dejavnosti, skupaj s pametnimi hevristikami in signali za grožnje, da prepozna zlonamerne datoteke. Glejte [ATP za SharePoint, OneDrive in Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).