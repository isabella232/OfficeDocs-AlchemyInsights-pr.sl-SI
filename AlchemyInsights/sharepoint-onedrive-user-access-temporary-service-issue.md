---
title: Težave z učinkovitostjo delovanja – SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771260"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ali OneDrive počasno, nedostopno ali ni na voljo za več uporabnikov

Če OneDrive ali SharePointovo mesto ni na voljo za več uporabnikov, ki so prej imeli dostop, je morda prišlo do začasne težave s storitvijo. [Preverite nadzorno ploščo za stanje storitve](https://portal.office.com/adminportal/home#/servicehealth).

**Dodajanje in licenciranje uporabnika**

Zagotovite, da [dodelite licence uporabnikom v storitvi Microsoft 365 za podjetja](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Dodeljevanje dovoljenj**

Če je uporabniku dodeljena SharePointova licenca in še vedno prejema sporočilo o zavrnjenem dostopu, zagotovite, da je dodeljena [ustrezna raven dovoljenj](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Razmislite o uporabi funkcije zahteve za dostop**

[Funkcija zahteve za dostop](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) osebam omogoča, da zahtevajo dostop do vsebine, ki je trenutno nimajo dovoljenja za ogled.

**Dovoli skript po meri, lahko povzroči težave z zavrnjenim dostopom**

Obstajajo določeni scenariji, kjer lahko funkcija *skripta za dovolitev po meri* predstavlja dostop zavrnjen. Seznam funkcij, ki so na voljo, varnostna opozorila in možnost onemogočanja funkcije. Obiščite [Dovoli ali preprečite skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

