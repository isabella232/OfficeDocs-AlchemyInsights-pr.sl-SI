---
title: Skrbniško središče za Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354104"
---
# <a name="teams-admin-center"></a>Skrbniško središče za Teams

Več informacij o upravljanju aplikacije Teams v [Skrbniškem središču za Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Če ne morete dostopati do Skrbniškega središča za Teams, preverite te elemente:

- Prepričajte se, da ste omogočili ustrezne [naslove IP in URL-je za Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v katerih koli napravah nadziranega podomrežja (požarni zid itd.) ali pravilih požarnega zidu v lokalnem računalniku.
- Prepričajte se, da se podatki za prijavo, s katerimi dostopate do Skrbniškega središča za Teams, ujemajo z uporabniškim imenom na [Portalu za skrbnike za Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Če uporabniki niso prikazani v Skrbniškem središču za Teams, preverite te elemente:

- Ali ste ustvarili uporabnike oziroma dodelili licence v zadnjih 24 urah? Počakajte najmanj 24 ur, preden ustvarite vstopnico za podporo.
- Prepričajte se, da se dodelili ustrezne licence.
- Če imate krajevni imenik Active Directory, preverite, [ali je vrednost msRTCSIP-PrimaryUserAddress ali naslov SIP v polju» ProxyAddresses «v lokalnem imeniku Active Directory edinstven in oblika ustreza](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**uporabniško ime** uporabnika iz [skrbniškega središča Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Če nameravate obdržati Skype za podjetja Server uvajanje in so uporabniki homed na mestu uporabe in online: sledite **"Nastavi hibrid s Teams in Skype za podjetja online"** v vašem Skype za podjetja Server Control Panel in premikanje uporabnikov online.
