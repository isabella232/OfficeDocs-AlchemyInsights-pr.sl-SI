---
title: Teţave pri povezavi SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508439"
---
# <a name="sharepoint-designer-connection-issues"></a>Teţave pri povezavi SharePoint Designer 

Če program SharePoint Designer je težave povezave na SharePointovih mestih, poskusite naslednje skupne rešitve.

1. korak: Preverite, da SharePoint Designer 2013 posodobljen s [servisnim paketom SP1 za SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) in [2 avgust 2016 posodobite SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. korak: Jasno lokalnega predpomnilnika datotek:

1. Zaprite SharePoint Designer 2013.

2. V lokalnem računalniku, odstranite vse datoteke, ki so v vsakem od teh map.

    - %AppData%\Microsoft\Web strežnik Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Odprite SharePoint Designer 2013 in vnesite konto spet, da vidim, če deluje.

Korak 3: [omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Korak 4: Administratorji morali **Omogočajo skript po meri** v postavljanje SharePoint Admin Center omogočiti povezavo programa SharePoint Designer. Glej [Dovoli ali prepreči skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) za več informacij.


