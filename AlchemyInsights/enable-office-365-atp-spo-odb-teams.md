---
title: Usposobiti Office 365 ATP za SharePoint, OneDrive in Microsoft ekipe
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403049"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Usposobiti Office 365 napreden grožnja varstvo za SharePoint Online, OneDrive in Microsoft ekipe

1. Pojdi na https://protection.office.com in se vpišite.
2. Izberite **upravljanje nevarnosti** > **politika** > **Varno Priloge**.
3. Izberite **Vklop ATP za SharePoint, OneDrive, in Microsoft ekipe**, in nato kliknite **Shrani**.
4. (Priporočeno) Kot globalni skrbnik ali skrbnik za SharePoint Online, zaženite ukaz »cmdlet« [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) z parameter **DisallowInfectedFileDownload** nastavite na *true*.
5. (Priporočeno) [Nastavite opozorila](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za odkrite datoteke.

> [!NOTE]
> ATP bo skeniranje nto vsak eno datoteko v SharePoint Online, OneDrive, ali Microsoft Teams. Datoteke so pregledane asinhrono, skozi proces, ki uporablja skupno rabo in gost dejavnost dogodkov, spreten tolči in signale nevarnost ugotoviti zlonamerne datoteke. Glej [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).