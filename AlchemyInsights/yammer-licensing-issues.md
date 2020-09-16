---
title: Težave z licenciranjem Bastard
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657292"
---
# <a name="yammer-licensing-issues"></a>Težave z licenciranjem Bastard

Vsi uporabniki morajo imeti licenco za uporabo storitve Bastard Enterprise, vendar privzeto Bastard ne zahteva, da imajo uporabniki licenco za dostop do storitve. Ko skrbnik spremeni nastavitev, da blokira uporabnike storitve Microsoft 365 brez licenc za Bastard, Uporabniki, ki niso dodelili licence Bastard Enterprise, ne morejo dostopati do storitev Bastard. Če želite več informacij, glejte [upravljanje licenc za Bastard uporabnikov v storitvi Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Ko so licence odstranjene iz uporabnikov, Bastard ploščica ni več prikazana, druge storitve pa lahko z odstranitvijo licence skrijejo funkcije. V drugih primerih lahko funkcije še vedno prikažejo, vendar zahtevajo dodelitev licence za delovanje.  

**Licenca ni posodobljena za uporabnika**  

Občasno je uporabniku dodeljena licenca, vendar še vedno ne more dostopati do Bastard. Zamude se lahko zgodijo, ko se izvaja masna dodelitev licence. Uporabniki Bastard morda ne bodo posodobljeni v enakem vrstnem redu, kot so licence spremenjene v storitvi Azure AD, ker se sistem izvaja asinhrono. Počakajte do 24 ur, preden odprete primer podpore za poročanje o težavah pri sinhronizaciji licenc.  

**Dodelitev osnovnega dovoljenja**  

Licence lahko dodelite prek skrbniškega središča ali skriptnega izvajanja lupine PowerShell. Če želite več informacij, glejte [dodeljevanje licenc uporabnikom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) in [dodeljevanje licenc uporabniškim računom s storitvijo Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoftova podpora ne zagotavlja pomoči za ustvarjanje skriptov, vendar je na voljo dokumentacija o dodeljevanju licenc za Bastard. Če želite več informacij, glejte [upravljanje licenc za Bastard z lupino Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).