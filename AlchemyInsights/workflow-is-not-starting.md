---
title: Potek dela se ne začenja
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766113"
---
# <a name="workflow-is-not-starting"></a>Potek dela se ne začenja

- Poteki dela SharePoint 2010 in SharePoint 2013 se ne začenjajo.

    - Če se potek dela ne začne, lahko pride do začasne težave s storitvijo, kjer lahko uporabniki občasno povzročijo zamude pri poteku dela. Če želite preveriti, ali je vaša organizacija vplivala, preverite [Nadzorna plošča storitve](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .

    - Če je minilo več kot 24 ur, odkar ste prvič videli to težavo, prosimo, prijavite vozovnico za podporo. V mnogih primerih že delamo na rešitvi. Prosimo, dajte nam vsaj 24 ur, da dokončate rešitev.

- Poteki dela SharePoint 2010 so bili ob zagonu zakasnjeni.

    - To se zgodi, če je potek dela sprožen v velikih serijah. (na primer, ko je več elementov dodanih naenkrat).

    - Poteki dela niso zasnovani za zagon v realnem času, zato je zakasnitev po-design vedenje.

   -  Če je potek dela kompleksen Extensible Object Markup Language (XMOL), lahko kompilacija je počasna. Preverite [ta](https://support.microsoft.com//kb/3043697) članek.

    - Potek dela ali preoblikovanje je treba poenostaviti z vrsto platforme Microsoft SharePoint 2013 Workflow.

    - Če se je zgodovina poteka dela povečala, boste morda želeli Počisti elemente ali ustvariti nov seznam zgodovine.

        Več informacij: [purge zgodovina poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Sorodne teme
Želite poskusiti Microsoft Flow v SharePoint online?
- [Ustvari potek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


