---
title: Yammer težav z licenciranjem
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989751"
---
# <a name="yammer-licensing-issues"></a>Yammer težav z licenciranjem

Vsi uporabniki morajo imeti licenco za uporabo storitve Yammer Enterprise, vendar Yammer privzeto ne zahteva, da imajo uporabniki licenco za dostop do storitve. Ko skrbnik spremeni nastavitev in tako blokira Microsoft 365 uporabnikom brez Yammer licenc, uporabniki, ki jim licenca Yammer Enterprise ni bila dodeljena, ne morejo dostopati do Yammer storitve. Če želite več informacij, [glejte Yammer uporabniških licenc v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Ko uporabnikom odstranite licence, ploščica Yammer prikazana, druge storitve pa lahko za skrivanje funkcij uporabijo odstranjevanje licenc. V drugih primerih so lahko funkcije še vedno prikazane, vendar morate za upravljanje zahtevati dodelitev licence.  

**Licenca za uporabnika se ne posodablja**  

Občasno je uporabniku dodeljena licenca, vendar še vedno ne more dostopati do Yammer. Do zakasnitev pride, ko poteka množična dodelitev licenc. Yammer uporabniki morda ne bodo posodobljeni v enakem vrstnem redu, kot so licence spremenjene v imeniku Azure AD, ker se sistem izvaja asinhrono. Počakajte do 24 ur, preden odprete primer podpore, da prijavite težave s sinhronizacijo licenc.  

**Skupinsko dodeljevanje licenc**  

Licence lahko dodelite prek skrbniškega središča ali skriptnega izvajanja PowerShell. Če želite več informacij, [glejte Dodeljevanje licenc uporabnikom in](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Dodeljevanje licenc uporabniškim računom s Office 365 [PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsoftova podpora ne zagotavlja pomoči pri ustvarjanju skriptov, vendar je na voljo dokumentacija Yammer dodelitev licence. Če želite več informacij, [glejte Yammer licenc za uporabo storitve Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).