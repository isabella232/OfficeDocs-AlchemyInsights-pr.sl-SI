---
title: Težave pri vpisu v Microsoft 365 apps
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579917"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="875d9-102">Prazen vpisni zaslon v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="875d9-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="875d9-103">Če želite odpraviti to težavo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="875d9-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="875d9-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="875d9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="875d9-105">Ponastavi možnosti Internet Explorerja: pojdite na **Orodja**  >  **Internetne možnosti**  >  **Napredno**  >  **ponastavitev nastavitev Internet Explorerja** (upoštevajte, da boste izgubili nastavitve po meri) in se nato znova poskusite prijaviti v Office.</span><span class="sxs-lookup"><span data-stu-id="875d9-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="875d9-106">Onesposobiti okno zagovornik uporaba zaščita (WDAG) ali poljuben sličen močno žganje ali smešen-kačji strup disciplinski nadzornik v Oxfordu ali Cambridgeu:</span><span class="sxs-lookup"><span data-stu-id="875d9-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="875d9-107">Na nadzorni plošči pojdite v **programe**in izberite **Vklopi ali izklopi funkcije sistema Windows**.</span><span class="sxs-lookup"><span data-stu-id="875d9-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="875d9-108">Če je Windows Defender Application Guard omogočen, ga poskusite onemogočiti.</span><span class="sxs-lookup"><span data-stu-id="875d9-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="875d9-109">**Opomba:** Morda boste morali znova zagnati računalnik.</span><span class="sxs-lookup"><span data-stu-id="875d9-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="875d9-110">Zavarovati to mikroskop. AAD. Brokerčep [AAD WAM čep-v](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) je ne bitje tnalo z poljuben uporaba ali močno žganje/smešen-kačji strup disciplinski nadzornik v Oxfordu ali Cambridgeu.</span><span class="sxs-lookup"><span data-stu-id="875d9-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="875d9-111">[Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.</span><span class="sxs-lookup"><span data-stu-id="875d9-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="875d9-112">**Opomba:** Registrske poti za Office 2016 so se spremenile v 16,0.</span><span class="sxs-lookup"><span data-stu-id="875d9-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="875d9-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="875d9-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="875d9-114">Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi v Office 2016 graditi 16.0.7967 v operacijskem sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="875d9-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>