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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056506"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Ali v outlooku ni bilo mogoče najti Outlook v spletu?

Če uporabljate Outlook v spletu in se prikaže  sporočilo o napaki, da nabiralnika ni bilo mogoče najti, račun, ki ste ga uporabili za vzpostavljanje povezave s storitvijo Outlook v spletu, nima licence za Exchange Online, zato z računom ni povezan noben nabiralnik. Vaš skrbnik lahko dodeli licenco računu tako, da upošteva te korake:

1. Odprite [Skrbniško središče za Microsoft 365](https://portal.office.com/adminportal/home#/homepage) in pojdite na **Aktivni** uporabniki  v razdelku Uporabniki ter izberite uporabnika, ki vidi napako.

2. Na strani uporabnika, ki se  odpre, pojdite v razdelek  Licence in aplikacije, izberite ustrezno vrednost Lokacija in dodelite licenco, ki vsebuje Exchange Online (razširite licenco, da si ogledate podrobnosti o njem). Ko končate, kliknite **Shrani spremembe.**

Če je licenca v nekaterih primerih že dodeljena uporabniškem računu, lahko z odstranitvijo in ponovno dodelitevm licence odpravite težavo in jo pravilno uporabljate v sistemu: 

- Preverite, ali so vaše naročnine na M365 Exchange Online (in druge, če imate) trenutne in še niso pred kratkim potekle.

Ko ste prepričani, da naročnina ni potekla in da je bila uporabniškeu računu dodeljena veljavna licenca, lahko traja do 24 ur, da je licenca omogočana, zato boste morali morda počakati, da se težava odpravi. Če želite več informacij, [glejte Dodeljevanje in upravljanje licenc.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)