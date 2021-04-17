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
# <a name="teams-admin-center"></a><span data-ttu-id="80e93-102">Skrbniško središče za Teams</span><span class="sxs-lookup"><span data-stu-id="80e93-102">Teams Admin Center</span></span>

<span data-ttu-id="80e93-103">Več informacij o upravljanju aplikacije Teams v [Skrbniškem središču za Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="80e93-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="80e93-104">Če ne morete dostopati do Skrbniškega središča za Teams, preverite te elemente:</span><span class="sxs-lookup"><span data-stu-id="80e93-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="80e93-105">Prepričajte se, da ste omogočili ustrezne [naslove IP in URL-je za Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v katerih koli napravah nadziranega podomrežja (požarni zid itd.) ali pravilih požarnega zidu v lokalnem računalniku.</span><span class="sxs-lookup"><span data-stu-id="80e93-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="80e93-106">Prepričajte se, da se podatki za prijavo, s katerimi dostopate do Skrbniškega središča za Teams, ujemajo z uporabniškim imenom na [Portalu za skrbnike za Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="80e93-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="80e93-107">Če uporabniki niso prikazani v Skrbniškem središču za Teams, preverite te elemente:</span><span class="sxs-lookup"><span data-stu-id="80e93-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="80e93-108">Ali ste ustvarili uporabnike oziroma dodelili licence v zadnjih 24 urah?</span><span class="sxs-lookup"><span data-stu-id="80e93-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="80e93-109">Počakajte najmanj 24 ur, preden ustvarite vstopnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="80e93-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="80e93-110">Prepričajte se, da se dodelili ustrezne licence.</span><span class="sxs-lookup"><span data-stu-id="80e93-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="80e93-111">Če imate imenik Active Directory na mestu uporabe, preverite, ali je vrednost [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ali naslov SIP v polju ProxyAddresses v lokalnem imeniku Active Directory enolična in da se oblika zapisa ujema s **sip:** Uporabniško ime uporabnika v skrbniškem središču za Microsoft [365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="80e93-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="80e93-112">Če nameravate še naprej uporabljati uvajanje Skypa za podjetja Server in želite, da uporabniki uporabljajo storitve homed na mestu uporabe in Online: v nadzorni plošči strežnika Skype za podjetja Server upoštevajte »Nastavitev hibridnega uvajanja s storitvijo Teams in Skype za podjetja **Online«** in premaknite uporabnike v spletu.</span><span class="sxs-lookup"><span data-stu-id="80e93-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
