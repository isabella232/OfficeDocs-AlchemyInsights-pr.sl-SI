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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530906"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Potek dela email ne pošiljajo v SharePointov seznam ali knjižnico

1. Email s poteki dela se ne pošljejo vse uporabnike ali samo določenim uporabnikom, ali vidite napake **e-poštnega sporočila ni mogoče poslati. Preverite, ali je e-mail veljaven prejemnik**.

    Preverite, če uporabnik obstaja v skupini **Vse ljudi** dovoljenja (seznam informacij uporabnik) za to zbirko mest.  Vzorec neposredno URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Če uporabnik ne obstaja, se prepričajte, uporabnik je podpisal stran. 
    - Če gre za zunanjega uporabnika, se prepričajte, da njihovo povabilo sprejme.
    - Če uporabnik obstaja v skupini dovoljenja, poskrbite, da naslov ni pravilen.
    - Če uporabniki e-poštni naslov ni nastavljena tukaj, ustvarite vzorec Opozorilo za tega uporabnika, ki sili sinhronizacijo uporabniški račun od uporabnikov profil SharePoint v tej zbirki mest.
 
2. Email s poteki dela pošiljajo skrbniki zbirke ne pa drugim uporabnikom in vidim napako **HTTP prepovedano za <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Glej [Dostop zavrnjen, ko pošljete e-poštno skupino SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Prav tako, preverite, ali funkcija zbirke mest **dostop omejen uporabnik dovoljenje lockdown način** ni aktivna.


## <a name="related-topics"></a>Sorodne teme
Želite poskusiti Microsoft Flow v SharePoint Online?
- [Ustvari tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint in pretok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


