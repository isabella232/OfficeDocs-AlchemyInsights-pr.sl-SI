---
title: Potek dela se ne začne
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403759"
---
# <a name="workflow-is-not-starting"></a>Potek dela se ne začne

- Poteki dela v strežnikih SharePoint 2010 in SharePoint 2013 se ne začnejo.

    - Če se potek dela ne začne, je morda prišlo do začasne težave storitve, kjer lahko uporabniki pride do začasnih zakasnitev pri poteku dela. Na nadzorni [plošči s stanjem](https://admin.microsoft.com/AdminPortal/Home/servicehealth) storitve preverite, ali je to v vaši organizaciji vplivalo.

    - Če je od prve težave minilo več kot 24 ur, zabeležite vstopnico za podporo. V številnih primerih že delamo na rešitvi. Če želite dokončati rešitev, nam dajte vsaj 24 ur.

- Poteki dela v programu SharePoint 2010 so na začetku zakasnjeni.

    - Do tega pride, če se potek dela sproži v velikih paketih. (če je na primer dodanih več elementov hkrati).

    - Poteki dela niso načrtovani za izvajanje v realnem času, zato je zakasnitev privzeto vedenje.

   -  Če je potek dela zapleten, je zbiranje lahko počasno. Oglejte [si ta](https://support.microsoft.com//kb/3043697) članek.

    - Potek dela bi morali poenostaviti ali ga preoblikovati z vrsto platforme za poteke dela microsoft SharePoint 2013.

    - Če je zgodovina poteka dela več velika, boste morda želeli elemente očistiti ali ustvariti nov seznam zgodovine.

        Več informacij: [Čiščenje zgodovine poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Sorodne teme
Ali želite preskusiti Microsoft Flow v SharePoint Onlineu?
- [Create Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
