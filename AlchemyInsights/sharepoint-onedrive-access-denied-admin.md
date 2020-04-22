---
title: Odpravljanje težav s sporočili o zavrnitvi dostopa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758516"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Odpravljanje težav pri dostopu zavrnjen v SharePoint/OneDrive skrbniško središče

Če prejmete sporočilo o zavrnitvi dostopa, ko poskušate prebrskati do skrbniškega središča SharePoint/OneDrive, se prepričajte, da [uporabniku dodelite licenco](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Če ima uporabnik licenco, morate tudi poskrbeti, da jim je [dodeljena skrbniška vloga](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , ki lahko dostopa do skrbniških centrov.

Ta težava se lahko pojavi tudi, ko je uporabnik izbrisan in ponovno ustvarjen z istim glavnim uporabniškim imenom (UPN). Nov račun je ustvarjen z uporabo drugega PUID (Passport Enolični ID) vrednost. Ko uporabnik poskuša dostopati do zbirke mest ali njihove storitve OneDrive, ima uporabnik napačen PUID. Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto Active Directory (OU). Če so se uporabniki že prijavili v SharePoint, nato pa se premaknejo v drug OU in se znova sinhronizira s SharePointom, lahko to težavo izkusijo.

Če želite odpraviti to težavo, obnovite izvirno UPN s koraki v članku, [obnovite uporabnika v Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Opomba: Če v skrbniškem središču OneDrive ali SharePoint ni na voljo več uporabnikom, ki so že imeli dostop, lahko pride do začasne izdaje storitve.  [Preverite nadzorno ploščo za zdravje storitve](https://portal.office.com/adminportal/home#/servicehealth).


