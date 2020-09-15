---
title: Odpravljanje težav z dostopom do zavrnjenih sporočil v OneDrive za podjetja
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670632"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Odpravljanje težav z dostopom do zavrnjenih sporočil v OneDrive za podjetja

Do te težave pride, ko je uporabnik izbrisan in znova ustvarjen z istim glavnim imenom uporabnika (UPN). Nov račun je ustvarjen z uporabo drugega PUID (ID Passporta Unique). Ko uporabnik poskuša dostopati do zbirke mest ali njihove OneDrive, ima uporabnik nepravilen PUID. Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto imenika Active Directory (OU). Če so uporabniki že vpisani v SharePoint, nato pa so premaknjeni v drug OU in znova sinhronizirani s storitvijo SharePoint, lahko ta težava pride do te težave.

1. To težavo odpravite tako, da obnovite prvotni UPN s koraki v članku, [obnovite uporabnika v programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Če ne morete obnoviti prvotnega uporabnika, odstranite starega uporabnika iz mesta OneDrive s temi koraki, [odstranite uporabnika s seznama uporabnikovih informacij](). 
3. Ko je to storjeno, lahko preverite, ali ima uporabnik skrbniške pravice na spletnem mestu OneDrive, in sicer tako, da upošteva navodila za [Dodajanje skrbniškega OneDrive za uporabnika](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Če želite več informacij o ravneh dovoljenj, si oglejte članek [razumevanje ravni dovoljenj v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
