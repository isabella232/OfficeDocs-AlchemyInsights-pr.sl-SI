---
title: Odpravljanje težav dostop zavrnjen sporočila OneDrive za poslovne strani
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507827"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Odpravljanje težav dostop zavrnjen sporočila OneDrive za poslovne strani

Težavo se najpogosteje pojavi, ko uporabnik izbriše in ponovno ustvari z enakim glavnim imenom uporabnika (UPN). Novi račun je ustvarjen z uporabo različnih PUID (Passport Enolični ID) vrednost. Ko uporabnik poskuša za dostop do zbirke mest ali njihovih OneDrive, uporabnik je napačno PUID. Drugi scenarij vključuje sinhronizacija imenika z Active Directory organizacijska enota (OU). Če uporabniki so že vpisani v SharePoint, in nato preselil v različnih OU in resynced s SharePointom, da lahko pride do te težave.

1. Če želite težavo odpraviti obnovite izvirno UPN s korakom v članku,[obnoviti uporabnik v Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Če ne morete obnoviti izvirni uporabniki odstranite staro uporabnika s strani OneDrive, po teh korakih, [odstranite uporabnika iz seznamu informacij o uporabnikih](). 
3. Ko je to storjeno, lahko preverite, ali ima uporabnik admin pravice do OneDrive mesta po navodilih za [Dodajanje admin je za uporabnika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Več informacij na ravni dovoljenj, si oglejte članek, [razumevanje ravni dovoljenj v SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
