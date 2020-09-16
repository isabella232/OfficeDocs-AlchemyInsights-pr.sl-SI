---
title: E-pošta poteka dela ni poslana
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
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749005"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta poteka dela ni poslana za SharePointov seznam ali knjižnico

1. E-pošta iz potekov dela ni poslana vsem uporabnikom ali le določenim uporabnikom ali pa se prikaže sporočilo o napaki, da **e-poštnega sporočila ni mogoče poslati. Preverite, ali je e-pošta veljavna prejemnika**.

    Preverite, ali uporabnik obstaja v skupini dovoljenja za **vse osebe** (seznam uporabniških podatkov) za to zbirko mest.  Vzorčni neposredni spletni naslov: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Če uporabnik ne obstaja, se prepričajte, da je uporabnik vpisan na stran. 
    - Če gre za zunanjega uporabnika, se prepričajte, da je bilo njihovo povabilo sprejeto.
    - Če uporabnik obstaja v skupini» dovoljenja «, se prepričajte, da je e-poštni naslov pravilen.
    - Če e-poštni naslov za uporabnike ni nastavljen tukaj, ustvarite vzorčno Opozorilo za tega uporabnika, ki vsili sinhronizacijo tega uporabniškega računa iz uporabniških profilov SharePointa v to zbirko mest.
 
2. E-pošta iz potekov dela je poslana skrbnikom zbirke mest, ne pa tudi drugim uporabnikom in si oglejte napako **http <span>:</span>//URL/_vti_bin/Client.xvc.SP.utilities.Utility.SendEmail**.
 

    [Če želite poslati e-poštno sporočilo v SharePointovo skupino, si oglejte dostop zavrnjen](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Preverite tudi, ali funkcija zbirke mest z **omejenim dostopom za dovoljenje uporabnika** ni aktivna.


## <a name="related-topics"></a>Sorodne teme
Ali želite preskusiti Microsoft Flow v storitvi SharePoint online?
- [Ustvarjanje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


