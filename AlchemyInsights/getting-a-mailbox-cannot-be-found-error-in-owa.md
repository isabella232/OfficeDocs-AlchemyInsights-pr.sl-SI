---
title: 126 Ali v programu OWA ni mogoče najti napake o nabiralniku?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426678"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Ali v Outlooku v spletu ni bilo mogoče najti napake nabiralnika?

Če uporabljate Outlook v spletu in  se prikaže sporočilo o napaki Nabiralnika ni bilo mogoče najti, račun, ki ste ga uporabili za povezovanje z Outlookom v spletu, nima licence za Exchange Online, zato z računom ni povezan noben nabiralnik. Vaš skrbnik lahko dodeli licenco računu tako, da upošteva te korake:

1. Odprite  [Skrbniško središče za Microsoft 365](https://portal.office.com/adminportal/home#/homepage)  in pojdite na Aktivni uporabniki v razdelku Uporabniki ter izberite uporabnika, ki vidi napako.

2. Na strani uporabnika, ki se  odpre, pojdite v razdelek  Licence in aplikacije, izberite ustrezno vrednost Lokacija in dodelite licenco, ki vsebuje Exchange Online (razširite licenco, da si ogledate njene podrobnosti). Ko končate, kliknite **Shrani spremembe.**

Če je licenca v nekaterih primerih že dodeljena uporabniškem računu, lahko z odstranitvijo in ponovno dodelitevm licence odpravite težavo in jo pravilno uporabljate v sistemu: 

- Preverite, ali so vaše naročnine na M365 Exchange Online (in druge, če so na voljo) trenutne in še niso pred kratkim potekle.

Ko ste prepričani, da naročnina ni potekla in da je bila uporabniškeu računu dodeljena veljavna licenca, lahko traja do 24 ur, da je licenca omogočana, zato boste morali morda počakati, da se težava odpravi. Če želite več informacij, [glejte Dodeljevanje in upravljanje licenc.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)