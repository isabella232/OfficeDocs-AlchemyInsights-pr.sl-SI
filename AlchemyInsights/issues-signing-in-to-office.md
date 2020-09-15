---
title: Težave pri vpisu v programe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695303"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="34e65-102">Prazen zaslon za vpis v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="34e65-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="34e65-103">Če želite odpraviti to težavo, naredite to:</span><span class="sxs-lookup"><span data-stu-id="34e65-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="34e65-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="34e65-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="34e65-105">Ponastavitev možnosti Internet Explorerja: pojdite v razdelek **Orodja**  >  **Internetne možnosti**  >  **Napredno**  >  **ponastavitev nastavitev Internet Explorerja** (upoštevajte, da boste izgubili nastavitve po meri), nato pa se poskusite znova vpisati v Office.</span><span class="sxs-lookup"><span data-stu-id="34e65-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="34e65-106">Onemogočite aplikacijo Guard (WDAG) programa Windows Defender ali kateri koli podoben požarni zid ali protivirusni program:</span><span class="sxs-lookup"><span data-stu-id="34e65-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="34e65-107">Na nadzorni plošči pojdite v razdelek **programi**in nato izberite **Vklopi ali izklopi funkcije sistema Windows**.</span><span class="sxs-lookup"><span data-stu-id="34e65-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="34e65-108">Če je omogočena zaščita programa Windows Defender, jo poskusite onemogočiti.</span><span class="sxs-lookup"><span data-stu-id="34e65-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="34e65-109">**Opomba:** Morda boste morali znova zagnati računalnik.</span><span class="sxs-lookup"><span data-stu-id="34e65-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="34e65-110">Zagotovite, da [vtičnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. zvočna WAM. BrokerPlugin ne blokira noben program ali požarni zid/protivirusni program.</span><span class="sxs-lookup"><span data-stu-id="34e65-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="34e65-111">[Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="34e65-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="34e65-112">**Opomba:** Poti registra za Office 2016 so se spremenile v 16,0.</span><span class="sxs-lookup"><span data-stu-id="34e65-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="34e65-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="34e65-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="34e65-114">Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi na Office 2016 Build 16.0.7967 v sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="34e65-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>