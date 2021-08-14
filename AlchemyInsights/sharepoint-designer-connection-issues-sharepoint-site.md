---
title: SharePoint Težave s povezavo oblikovalnika
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942041"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Težave s povezavo oblikovalnika 

Če SharePoint Designer ima težave s SharePoint spletnih mest, poskusite s spodnjimi pogostimi rešitvami.

1. korak: Preverite, ali je SharePoint Designer 2013 posodobljen s servisnim paketom [SharePoint Designer s servisnim](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) paketom SP1 in posodobitvijo z dne [2. avgusta 2016 za SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



2. korak: Počistite lokalne predpomnjene datoteke:

1. Zaprite SharePoint Designer 2013.

2. V lokalnem računalniku odstranite vse datoteke, ki jih najdete v vsaki od teh map.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Odprite SharePoint Designer 2013 in znova vnesite račun, da si ogledate, ali deluje.

3. korak: [Omogočanje sodobnega preverjanja pristnosti za Office 2013 v Windows napravah.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

4. korak: Skrbniki  bodo morali dovoliti skript po meri v skrbniškem središču SharePoint da omogočijo povezavo SharePoint Oblikovalnik. Če [želite več informacij, glejte Omogočanje ali preprečevanje](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) skripta po meri.


