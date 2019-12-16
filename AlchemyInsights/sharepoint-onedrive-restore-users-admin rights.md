---
title: Odpravljanje težav pri dostopu zavrnjen sporočila na spletna mesta OneDrive za podjetja
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051621"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Odpravljanje težav pri dostopu zavrnjen sporočila na spletna mesta OneDrive za podjetja

Ta težava se najpogosteje pojavi, ko je uporabnik izbrisan in ponovno ustvarjen z istim glavnim imenom uporabnika (UPN). Nov račun je ustvarjen z uporabo drugega PUID (Passport Enolični ID) vrednost. Ko uporabnik poskuša dostopati do zbirke mest ali njihove storitve OneDrive, ima uporabnik napačen PUID. Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto Active Directory (OU). Če so se uporabniki že prijavili v SharePoint, nato pa se premaknejo v drug OU in se znova sinhronizira s SharePointom, lahko to težavo izkusijo.

1. Če želite odpraviti to težavo, morate obnoviti izvirni UPN s koraki v članku, [obnovite uporabnika v Officeu 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Če prvotnega uporabnika ne morete obnoviti, odstranite starega uporabnika s spletnega mesta OneDrive s temi koraki, [odstranite uporabnika s seznama uporabniških podatkov](). 
3. Ko je to storjeno, lahko preverite, ali ima uporabnik skrbniške pravice do mesta OneDrive, tako da sledi korakom, da [dodate skrbnika za uporabnikovo storitev onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Če želite več informacij o ravneh dovoljenj, si oglejte članek, [razumevanje ravni dovoljenj v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
