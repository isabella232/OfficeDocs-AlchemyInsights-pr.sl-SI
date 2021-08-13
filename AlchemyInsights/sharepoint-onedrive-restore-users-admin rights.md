---
title: Odpravljanje težav z dostopom je zavrnjeno pošiljanje OneDrive za podjetja spletnih mest
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957809"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Odpravljanje težav z dostopom je zavrnjeno pošiljanje OneDrive za podjetja spletnih mest

Do te težave najpogosteje pride, ko izbrišete uporabnika in ga znova ustvarite z istim glavnim imenom uporabnika (UPN). Novi račun je ustvarjen z drugo vrednostjo PUID (Passport Unique ID). Ko uporabnik poskuša dostopati do zbirke mest ali zbirke OneDrive, ima uporabnik napačen PUID. Drugi primer vključuje sinhronizacijo imenika z enoto organizacije imenika Active Directory (OU). Če so uporabniki že vpisani v SharePoint, nato pa so premaknjeni v drugo OU in znova sinhronizirani s SharePoint, lahko pride do te težave.

1. Če želite odpraviti to težavo, morate obnoviti izvirni UPN z koraki v članku Obnovitev [uporabnika v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Če izvirnega uporabnika ne morete obnoviti, odstranite starega uporabnika s spletnega mesta OneDrive po teh korakih: Odstranite uporabnika s seznama [informacij o uporabniku.]() 
3. Ko je to narejeno, lahko preverite, ali ima uporabnik skrbniške pravice za spletno mesto OneDrive tako, da sledite korakom za dodajanje skrbniških pravic za [uporabnikovo OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Če želite več informacij o ravneh dovoljenj, si oglejte članek [Razumevanje ravni dovoljenj v SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
