---
title: E-pošta poteka dela ni poslana
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049389"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta poteka dela ni poslana za SharePointov seznam ali knjižnico

1. E-pošta iz potekov dela ni poslana vsem uporabnikom ali samo določenim uporabnikom ali pa se prikaže sporočilo o napaki, **da e-poštnega sporočila ni mogoče poslati. Preverite, ali ima e-pošta veljaven prejemnik**.

    Preverite, ali uporabnik obstaja v skupini dovoljenja za **vse ljudi** (seznam uporabniških informacij) za to zbirko mest.  Sample neposredni URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0

    - Če uporabnik ne obstaja, se prepričajte, da je uporabnik podpisan na strani. 
    - Če je zunanji uporabnik, se prepričajte, da je bilo njihovo povabilo sprejeto.
    - Če uporabnik v skupini dovoljenj obstaja, se prepričajte, da je e-poštni naslov pravilen.
    - Če uporabnik e-poštni naslov ni nastavljen tukaj, nato pa ustvarite vzorčno Opozorilo za tega uporabnika, ki prisili sinhronizacijo tega uporabniškega računa iz uporabniških profilov SharePoint v to zbirko mest.
 
2. E-pošta iz potekov dela se pošlje skrbnikom zbirke mest, ne pa tudi drugim uporabnikom, in si oglejte napako **http prepovedano <span>https:</span>//URL/_vti_bin/Client.xvc.SP.utilities.Utility.SendEmail**.
 

    [Če pošljete e-poštno sporočilo v SharePointovo skupino, glejte dostop zavrnjen](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Preverite tudi, ali je funkcija zbirke mest za **zaklepanje z omejenim dostopom uporabnika** neaktivna.


## <a name="related-topics"></a>Sorodne teme
Želite poskusiti Microsoft Flow v SharePoint online?
- [Ustvari potek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


