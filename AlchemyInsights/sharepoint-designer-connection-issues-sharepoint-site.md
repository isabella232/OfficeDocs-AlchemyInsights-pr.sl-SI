---
title: Ravni dovoljenj SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760708"
---
# <a name="sharepoint-designer-connection-issues"></a>Teţave pri povezavi SharePoint Designer 

Če program SharePoint Designer je težave povezave na SharePointovih mestih, prosim poskusite naslednje skupne rešitve.

1. korak: Preverite, ali je posodobiti SharePoint Designer.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer usluga zmašiti 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Posodobitev za SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

2. korak: Jasno lokalnega predpomnilnika datotek

- Zaprite SharePoint Designer 2013.

- V lokalnem računalniku, poiščite naslednje mape odstranite predpomnjene datoteke.

- Kliknite Start, Zaženi in izbrisati vse datoteke najdete v vseh je pod lokacijah.

Strežnik %AppData%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Odprite SharePoint Designer 2013 in vnesite konto spet, da vidim, če deluje.

Korak 3: [omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Korak 4: Administratorji morali omogočajo skript po meri omogočiti povezavo programa SharePoint Designer.

Podrobni koraki, primeri in vidiki glejte [Dovoli ali prepreči skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


