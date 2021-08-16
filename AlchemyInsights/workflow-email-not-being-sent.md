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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072536"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Workflow email is not being sent for a SharePoint list or library

1. E-pošta iz potekov dela ni poslana vsem uporabnikom ali le določenim uporabnikom ali pa se prikaže napaka E-poštnega sporočila ni mogoče poslati. Prepričajte se, da e-poštno sporočilo vključuje **veljavnega prejemnika.**

    Preverite, ali uporabnik obstaja v **skupini dovoljenj Vse osebe** (seznam informacij o uporabniku) za to zbirko mest.  Vzorčni url: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Če uporabnik ne obstaja, preverite, ali je uporabnik vpisan na stran. 
    - Če gre za zunanjega uporabnika, se prepričajte, da je bilo njihovo povabilo sprejeto.
    - Če uporabnik obstaja v skupini dovoljenj, preverite, ali je e-poštni naslov pravilen.
    - Če uporabniški e-poštni naslov ni nastavljen, ustvarite vzorčno opozorilo za tega uporabnika, ki prisili sinhronizacijo tega uporabniškega računa iz uporabniških profilov SharePoint v to zbirko mest.
 
2. E-pošta iz potekov dela je poslana skrbnikom zbirke mest, ne pa tudi drugim uporabnikom, ogled napake HTTP Prepovedano za **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Glejte [Dostop je zavrnjen, ko pošljete e-poštno sporočilo SharePoint skupini](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Poleg tega se prepričajte, da **funkcija zaklepa dovoljenja** za omejen dostop uporabnikov ni aktivna.


## <a name="related-topics"></a>Sorodne teme
Ali želite preskusiti Microsoft Flow spletnem SharePoint Onlineu?
- [Ustvarjanje Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


