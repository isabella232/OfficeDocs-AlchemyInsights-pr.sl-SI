---
title: Potek dela email ni poslan
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270688"
---
# <a name="workflow-email-is-not-being-sent"></a>Potek dela email ni poslan

1. Email s poteki dela se ne pošljejo vse uporabnike ali samo določenim uporabnikom, ali vidite napake **e-poštnega sporočila ni mogoče poslati. Preverite, ali je e-mail veljaven prejemnik**.

    Preverite, če uporabnik obstaja v skupini **Vse ljudi** dovoljenja (seznam informacij uporabnik) za to zbirko mest.  Vzorec neposredno URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Če uporabnik ne obstaja, se prepričajte, uporabnik je podpisal stran. 
    - Če gre za zunanjega uporabnika, se prepričajte, da njihovo povabilo sprejme.
    - Če uporabnik obstaja v skupini dovoljenja, poskrbite, da naslov ni pravilen.
    - Če uporabniki e-poštni naslov ni nastavljena tukaj, ustvarite vzorec Opozorilo za tega uporabnika, ki sili sinhronizacijo uporabniški račun od uporabnikov profil SharePoint v tej zbirki mest.
 
2. Email s poteki dela pošiljajo skrbniki zbirke ne pa drugim uporabnikom in vidim napako **HTTP prepovedano za <spam> <spam> ** <spam> <spam>.
 

    Glej [Dostop zavrnjen, ko sent email v skupine](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Prav tako, preverite, ali funkcija zbirke mest **dostop omejen uporabnik dovoljenje lockdown način** ni aktivna.


## <a name="related-topics"></a>Sorodne teme
Želite poskusiti Microsoft Flow v SharePoint Online?
- [Ustvari tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in pretok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


