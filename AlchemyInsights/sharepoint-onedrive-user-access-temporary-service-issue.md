---
title: Težave z učinkovitostjo SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093796"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ali OneDrive Slow, Nedostopen ali Nedostopen za več uporabnikov

Če spletno OneDrive ali SharePoint ni na voljo več uporabnikom, ki so prej imeli dostop, je morda prišlo do začasne težave s storitvijo. [Preverite nadzorno ploščo s stanjem storitve.](https://portal.office.com/adminportal/home#/servicehealth)

**Dodajanje in licenca uporabnika**

Prepričajte se, [da uporabnikom v podjetju Microsoft 365 licence.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Dodeljevanje dovoljenj**

Če je bila uporabniku dodeljena SharePointova licenca in še vedno prejme sporočilo o zavrnjenem dostopu, preverite, ali je mu dodeljena [ustrezna](https://docs.microsoft.com/sharepoint/understanding-permission-levels) raven dovoljenj.

**Razmislite o uporabi funkcije zahteve za dostop**

Funkcija [zahteve za dostop](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogoča ljudem, da zahtevajo dostop do vsebine, ki je trenutno ne želijo videti.

**Omogočanje skripta po meri lahko povzroči težave z dostopom je zavrnjen**

V nekaterih scenarijih funkcija za omogočanje *skripta po meri* morda predstavlja zavrnjen dostop. Seznam funkcij, na katere to vpliva, je treba upoštevati varnost in možnost onemogočanja funkcije. Obiščite [spletno mesto Dovoli ali prepreči skript po meri.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

