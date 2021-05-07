---
title: Uvajanje dodatkov za Programi Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233550"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Uvajanje dodatkov za Programi Microsoft 365

Centralizirana uvedba je priporočen način uvedbe dodatkov Office uporabnikom in skupinam znotraj organizacije. Če želite uvesti dodatke, upoštevajte spodnja navodila:

**Opomba:** Če želite namestiti dodatke za Office kot posamezen uporabnik, glejte Ogled, upravljanje in namestitev dodatkov [v Office programih.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Poleg tega poskrbite, da Office omogočene individualne pridobitve dodatkov iz Trgovine. Če želite več informacij, glejte Preprečevanje prenosov dodatkov tako, da izklopite Office Store za vse [odjemalce (razen za Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Zagotovite, da vaše okolje izpolnjuje zahteve za uvedbo dodatkov s centralizirano uvedbo. Če želite več informacij, glejte [Zahteve.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Če želite **Nastavitve**  >  **dodatke,** si  >  **v** skrbniškem središču Microsoft 365 Office 2016 Microsoft 365 Pridobite aplikacije. 

Opombe: 

- Integrirani programi zahtevajo, da ima skrbnik dovoljenja globalnega skrbnika Exchange skrbnika.

- Ko uvajate dodatke za več uporabnikov, priporočamo, da za dodelitve uporabite skupine namesto posameznih uporabnikov. Če želite več [informacij, glejte Kaj je treba upoštevati pri dodeljevanju dodatka uporabnikom in skupinam.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centralizirana uvedba ne podpira uporabnikov v ugnezdenih skupinah ali skupinah, ki imajo nadrejene skupine. Če želite več informacij, [glejte Dodelitve uporabnikov in skupin.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Zagotovite, da je storitev za upravljanje Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogočena za uporabnike, da se vpišejo. Če želite več informacij, [glejte Konfiguracija lastnosti aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Če pride do težav pri uvajanju dodatkov z integriranimi programi, jih poskusite [uvesti z dodatki.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Če želite več informacij, si oglejte:

[Uvajanje dodatkov v skrbniškem središču](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje dodatkov v skrbniškem središču](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Uporaba ukazov »cmdlet« PowerShell](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) za centralizirano uvedbo za upravljanje dodatkov 
 [Objavljanje Office dodatkov s centralizirano uvedbo prek skrbniškega središča Microsoft 365 za Office](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Odpravljanje težav: Uporabnik ne vidi dodatkov](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Odpravljanje napak uporabnikov Office dodatkov](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)