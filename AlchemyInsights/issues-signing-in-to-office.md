---
title: Težave pri vpisu v aplikacije Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833055"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="80f3c-102">Prazen zaslon za vpis v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="80f3c-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="80f3c-103">Če želite odpraviti to težavo, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="80f3c-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="80f3c-104">Namestite najnovejše posodobitve za [Windows in](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="80f3c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="80f3c-105">Ponastavitev možnosti v Internet Explorerju: Pojdite na Orodja za internetne možnosti Napredne nastavitve  >    >    >  **Internet Explorerja** (upoštevajte, da boste izgubili nastavitve po meri) in se nato znova poskusite vstaviti v Office.</span><span class="sxs-lookup"><span data-stu-id="80f3c-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="80f3c-106">Onemogočite Windows Defender Application Guard (WDAG) ali podoben požarni zid ali protivirusni program:</span><span class="sxs-lookup"><span data-stu-id="80f3c-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="80f3c-107">Na nadzorni plošči izberite **Programi in** nato vklop ali izklop funkcij **sistema Windows.**</span><span class="sxs-lookup"><span data-stu-id="80f3c-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="80f3c-108">Če je windows Defender Application Guard omogočen, ga poskusite onemogočiti.</span><span class="sxs-lookup"><span data-stu-id="80f3c-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="80f3c-109">**Opomba:** Morda boste morali znova zagnati računalnik.</span><span class="sxs-lookup"><span data-stu-id="80f3c-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="80f3c-110">Prepričajte se, da nobenega programa ali požarnega zidu/protivirusnega programa ne blokira vtičnika Microsoft.AAD.Plugin [AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)</span><span class="sxs-lookup"><span data-stu-id="80f3c-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="80f3c-111">[Počistite poverilnice za Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="80f3c-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="80f3c-112">**Opomba:** Poti registra za Office 2016 so se spremenile v 16.0.</span><span class="sxs-lookup"><span data-stu-id="80f3c-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="80f3c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="80f3c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="80f3c-114">Če želite več informacij, glejte Težave pri vpisu s povezavo po posodobitvi na [gradovi Office 2016, graden 16.0.7967 v sistemu Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="80f3c-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>