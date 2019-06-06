---
title: Uporabnikom dostop do SharePoint in OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736663"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Uporabnikom dostop do SharePoint in OneDrive

Težavo se najpogosteje pojavi, ko uporabnik izbriše in ponovno ustvari z enakim glavnim imenom uporabnika (UPN). Novi račun je ustvarjen z uporabo različnih PUID (Passport Enolični ID) vrednost. Ko uporabnik poskuša za dostop do zbirke mest ali njihovih OneDrive, uporabnik je napačno PUID. Drugi scenarij vključuje sinhronizacija imenika z Active Directory organizacijska enota (OU). Če uporabniki so že vpisani v SharePoint, in nato preselil v različnih OU in resynced s SharePointom, da lahko pride do te težave.

Če želite težavo odpraviti obnovite izvirno UPN s korakom v članku,[obnoviti uporabnik v Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

Ko je to storjeno, lahko preverite, ali ima uporabnik admin pravice do OneDrive mesta po navodilih za [Dodajanje admin je za uporabnika OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Več informacij na ravni dovoljenj, si oglejte članek, [razumevanje ravni dovoljenj v SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
