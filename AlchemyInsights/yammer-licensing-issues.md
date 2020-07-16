---
title: Težave z izdajanjem licenc za yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148321"
---
# <a name="yammer-licensing-issues"></a>Težave z izdajanjem licenc za yammer

Vsi uporabniki morajo imeti licenco za uporabo storitve Yammer Enterprise, vendar storitev Yammer privzeto ne zahteva, da imajo uporabniki licenco za dostop do storitve. Ko skrbnik spremeni nastavitev, da blokira Microsoft 365 uporabnike brez licenc Yammer, Uporabniki, ki niso dodelili licence Yammer Enterprise, ne morejo dostopati do storitve Yammer. Če želite več informacij, glejte [upravljanje uporabniških licenc za Yammer v Officeu 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Ko so licence odstranjene iz uporabnikov, ploščica Yammer ni več prikazana, druge storitve pa lahko za skrivanje funkcij uporabljajo odstranjevanje licenc. V drugih primerih so funkcije še vedno lahko prikazane, vendar zahtevajo dodelitev licence za delovanje.  

**Licenca se ne posodablja za uporabnika**  

Občasno je uporabniku dodeljena licenca, vendar še vedno ne more dostopati do Yammer. Zamude so verjetneje nastale, ko se izvaja dodelitev množične licence. Uporabniki storitev yammer morda ne bodo posodobljeni v enakem vrstnem redu, kot so licence spremenjene v storitvi Azure AD, ker sistem deluje asinhrono. Počakajte do 24 ur, preden odprete primer podpore za poročanje o težavah s sinhronizacijo licenc.  

**Dodelitev licence v velikem obsegu**  

Licence lahko dodelite prek skrbniškega središča ali skriptov PowerShell. Če želite več informacij, glejte [dodeljevanje licenc uporabnikom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) in [dodeljevanje licenc uporabniškim računom z Officeom 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoftova podpora ne zagotavlja pomoči pri ustvarjanju skriptov, vendar je na voljo dokumentacija o dodelitvi licenc za licenco Yammer. Če želite več informacij, glejte [upravljanje licenc za Yammer z lupino Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).