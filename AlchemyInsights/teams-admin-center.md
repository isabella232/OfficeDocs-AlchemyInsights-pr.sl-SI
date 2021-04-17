---
title: Skrbniško središče za Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826395"
---
# <a name="teams-admin-center"></a>Skrbniško središče za Teams

Več informacij o upravljanju aplikacije Teams v [Skrbniškem središču za Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Če ne morete dostopati do Skrbniškega središča za Teams, preverite te elemente:

- Prepričajte se, da ste omogočili ustrezne [naslove IP in URL-je za Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v katerih koli napravah nadziranega podomrežja (požarni zid itd.) ali pravilih požarnega zidu v lokalnem računalniku.
- Prepričajte se, da se podatki za prijavo, s katerimi dostopate do Skrbniškega središča za Teams, ujemajo z uporabniškim imenom na [Portalu za skrbnike za Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Če uporabniki niso prikazani v Skrbniškem središču za Teams, preverite te elemente:

- Ali ste ustvarili uporabnike oziroma dodelili licence v zadnjih 24 urah? Počakajte najmanj 24 ur, preden ustvarite vstopnico za podporo.
- Prepričajte se, da se dodelili ustrezne licence.
- Če imate imenik Active Directory na mestu uporabe, preverite, ali je vrednost [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ali naslov SIP v polju ProxyAddresses v lokalnem imeniku Active Directory enolična in da se oblika zapisa ujema s **sip:** Uporabniško ime uporabnika v skrbniškem središču za Microsoft [365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Če nameravate še naprej uporabljati uvajanje Skypa za podjetja Server in želite, da uporabniki uporabljajo storitve homed na mestu uporabe in Online: v nadzorni plošči strežnika Skype za podjetja Server upoštevajte »Nastavitev hibridnega uvajanja s storitvijo Teams in Skype za podjetja **Online«** in premaknite uporabnike v spletu.
