---
title: Vprašanja, ki se vpisujete Office aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938343"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="4638a-102">Obrazec vpisni zaslon v Office aplikacije</span><span class="sxs-lookup"><span data-stu-id="4638a-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="4638a-103">Če želite odpraviti težavo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="4638a-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="4638a-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="4638a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="4638a-105">Ponastavite možnosti Internet Explorerja: iti k **rokodelsko orodje** > **Internetne možnosti** > **Advanced** > **Ponastavljanje nastavitev programa Internet Explorer** (upoštevajte, da boste izgubili nastavitve po meri) in nato poskusite vpisujete Office znova.</span><span class="sxs-lookup"><span data-stu-id="4638a-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="4638a-106">Onesposobiti okno zagovornik uporabe straže (WDAG) ali podoben program močno žganje ali smešen-kačji strup:</span><span class="sxs-lookup"><span data-stu-id="4638a-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="4638a-107">V nadzorni plošči, iti k **Programs**, in nato izberite **zavoj okno zunanja oblika naprej ali ne sveže**.</span><span class="sxs-lookup"><span data-stu-id="4638a-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="4638a-108">Če je omogočen Windows Defender uporabo straže, poskusite onemogočiti to.</span><span class="sxs-lookup"><span data-stu-id="4638a-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="4638a-109">**Opomba:** Boste morda morali ponovno zagnati računalnik.</span><span class="sxs-lookup"><span data-stu-id="4638a-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="4638a-110">Zagotoviti, da Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne bo blokirala vsak program ali požarni zid/smešen-kačji strup program.</span><span class="sxs-lookup"><span data-stu-id="4638a-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="4638a-111">[Jasno urad poverilnic](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.</span><span class="sxs-lookup"><span data-stu-id="4638a-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="4638a-112">**Opomba:** Registrske poti za Office 2016 spremenili v 16,0.</span><span class="sxs-lookup"><span data-stu-id="4638a-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="4638a-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="4638a-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="4638a-114">Če želite več informacij, glejte [te¾ave pri povezovanju v vpisno po posodobitvi za Office 2016 zidava 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="4638a-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>