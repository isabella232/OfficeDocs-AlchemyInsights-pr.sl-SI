---
title: Težave s povezavo za SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727187"
---
# <a name="sharepoint-designer-connection-issues"></a>Težave s povezavo za SharePoint Designer 

Če ima SharePoint Designer težave s povezavo do SharePointovih mest, poskusite s temi pogostimi rešitvami.

1. korak: Preverite, ali je SharePoint Designer 2013 posodobljen s [servisnim paketom SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) in [posodobitvijo avgusta 2, 2016 za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. korak: počistite lokalne datoteke predpomnilnika:

1. Zaprite SharePoint Designer 2013.

2. V lokalnem računalniku odstranite vse datoteke, ki so bile najdene v vsaki od teh map.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Odprite SharePoint Designer 2013 in znova vnesite račun, da preverite, ali deluje.

3. korak: [Omogočanje sodobnega preverjanja pristnosti za Office 2013 v napravah s sistemom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4. korak: skrbniki bodo morali **omogočiti skript po meri** v skrbniškem središču za SharePoint, da se omogoči povezava do SharePointovega oblikovalca. Če želite več informacij, glejte [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


