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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801091"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogočanje Microsoftovega zagovornika za Office 365 za SharePoint online, OneDrive in Microsoft Teams

1. Pojdite na https://protection.office.com in se vpišite.
2. Izberite **Threat management**  >  **Policy**  >  **varna Priloga** pravilnika za upravljanje groženj.
3. Izberite **Vklopi ATP za SharePoint, OneDrive in Microsoft Teams** in nato kliknite **Shrani** .
4. Priporočeno Kot globalni skrbnik ali skrbnik SharePoint Onlinea zaženite ukaz» cmdlet « [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** , nastavljenim na *True* .
5. Priporočeno [Nastavite opozorila](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za zaznane datoteke.

> [!NOTE]
> ATP bo pregledal vsako posamezno datoteko v storitvi SharePoint online, OneDrive ali Microsoft teams. Datoteke so asinhrono skenirane, in sicer s postopkom, ki uporablja dogodke skupne rabe in gostujoče dejavnosti, skupaj s pametnimi hevristikami in signali za grožnje, da prepozna zlonamerne datoteke. Glejte [ATP za SharePoint, OneDrive in Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).