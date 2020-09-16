---
title: Skrbniško središče za Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670380"
---
# <a name="teams-admin-center"></a>Skrbniško središče za Teams

Več informacij o upravljanju aplikacije Teams v [Skrbniškem središču za Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Če ne morete dostopati do Skrbniškega središča za Teams, preverite te elemente:

- Prepričajte se, da ste omogočili ustrezne [naslove IP in URL-je za Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v katerih koli napravah nadziranega podomrežja (požarni zid itd.) ali pravilih požarnega zidu v lokalnem računalniku.
- Prepričajte se, da se podatki za prijavo, s katerimi dostopate do Skrbniškega središča za Teams, ujemajo z uporabniškim imenom na [Portalu za skrbnike za Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Če uporabniki niso prikazani v Skrbniškem središču za Teams, preverite te elemente:

- Ali ste ustvarili uporabnike oziroma dodelili licence v zadnjih 24 urah? Počakajte najmanj 24 ur, preden ustvarite vstopnico za podporo.
- Prepričajte se, da se dodelili ustrezne licence.
- Če imate na voljo imenik Active Directory, preverite, [ali je vrednost msRTCSIP-PrimaryUserAddress ali naslov SIP v polju proxyAddresses v lokalnem imeniku Active Directory enolična in oblika zapisa](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**uporabniško ime** uporabnika iz [skrbniškega središča za Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Če nameravate ohraniti uvajanje strežnika Skype za podjetja in imeti na voljo uporabniki na mestu uporabe in v spletu: sledite razdelku **» Nastavitev hibrida z aplikacijami Teams in Skype za podjetja online «** v nadzorni plošči za Skype za podjetja in premikanje uporabnikov v spletu.
