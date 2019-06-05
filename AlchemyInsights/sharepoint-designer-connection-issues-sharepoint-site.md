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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716907"
---
# <a name="sharepoint-designer-connection-issues"></a>Teţave pri povezavi SharePoint Designer 

<p>Če program SharePoint Designer je težave povezave na SharePointovih mestih, prosim poskusite naslednje skupne rešitve.</p> <p><strong>Korak 1:</strong> <strong>Preverite, ali SharePoint Designer je posodobljen&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer usluga zmašiti 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Posodobitev za SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Korak 2:</strong> <strong>Počistite datoteke lokalnega predpomnilnika</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Zaprite SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">V lokalnem računalniku, poiščite naslednje mape odstranite predpomnjene datoteke.&nbsp;</li> <li style="font-weight: 400;">Kliknite <strong>Start -&gt; teči</strong> in izbrišite vse datoteke, ki so na voljo na vseh je pod lokacijah.&nbsp;<br /><br />%AppData%\Microsoft\Web strežnik Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Odprite SharePoint Designer 2013 in vnesite konto spet, da vidim, če deluje.</li> </ol> <p><strong>Korak 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt</strong></a>&nbsp;</p> <p><strong>Korak 4:</strong> <strong>Administratorji morali dovoliti skript po meri omogočiti povezavo SharePoint Designer</strong>.</p> <p>Podrobni koraki, primeri in vidiki glejte <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Dovoli ali prepreči skript po meri</a>.&nbsp;</p>


