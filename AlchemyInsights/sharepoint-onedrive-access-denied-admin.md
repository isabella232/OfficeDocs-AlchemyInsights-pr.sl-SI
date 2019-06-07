---
title: Odpravljanje težav s postranski tajivec vest
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760356"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Odpravljanje težav s postranski tajivec sporočil v skrbniškem središču za Sharepoint/OneDrive

Če prejmete sporočilo o zavrnjenem ko poskušate brskati za Sharepoint/OneDrive Admin Center dostopu, prepričajte se, da vam [dodeli dovoljenje za uporabnika](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Če ima uporabnik dovoljenje, prav tako se prepričajte, so [dodeljena skrbniška vloga](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) ki lahko dostop do admin centri.

Ta težava se lahko pojavi tudi, ko uporabnik izbriše in ponovno ustvari z enakim glavnim imenom uporabnika (UPN). Novi račun je ustvarjen z uporabo različnih PUID (Passport Enolični ID) vrednost. Ko uporabnik poskuša za dostop do zbirke mest ali njihovih OneDrive, uporabnik je napačno PUID. Drugi scenarij vključuje sinhronizacija imenika z Active Directory organizacijska enota (OU). Če uporabniki so že vpisani v SharePoint, in nato preselil v različnih OU in resynced s SharePointom, da lahko pride do te težave.

Če želite težavo odpraviti, obnovite izvirno UPN s korakom v članku, [obnoviti uporabnik v Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Opomba: Če je OneDrive ali SharePoint Admin center ni na voljo za več uporabnikov, ki so prej imeli dostopa, lahko pride začasno storitev vprašanje.  [Preverite zdravje Nadzorna plošča storitev](https://portal.office.com/adminportal/home#/servicehealth).


