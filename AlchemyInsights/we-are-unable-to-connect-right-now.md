---
title: Težava z aktiviranjem – trenutno se ne moremo povezati
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725999"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="bf2cf-102">Popravljanje programa Microsoft 365 apps» trenutno se ne moremo povezati s sporočilom «</span><span class="sxs-lookup"><span data-stu-id="bf2cf-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="bf2cf-103">Če prejmete to sporočilo, naredite to:</span><span class="sxs-lookup"><span data-stu-id="bf2cf-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bf2cf-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve strežnika proxy, da potrdite, da ne blokirajo internetnega dostopa do programov Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bf2cf-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bf2cf-105">Oglejte si [Microsoftove URL-je in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bf2cf-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bf2cf-106">Pojdite na **začetek**  >  **Zaženi**in vnesite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="bf2cf-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bf2cf-107">Zagotovite, da se izvajajo te storitve:</span><span class="sxs-lookup"><span data-stu-id="bf2cf-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bf2cf-108">Samodejna nastavitev omrežnih naprav, povezanih z omrežjem</span><span class="sxs-lookup"><span data-stu-id="bf2cf-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bf2cf-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="bf2cf-109">Network List Service</span></span>
    - <span data-ttu-id="bf2cf-110">Poznavanje omrežnega mesta</span><span class="sxs-lookup"><span data-stu-id="bf2cf-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bf2cf-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="bf2cf-111">Windows Event Log</span></span>

<span data-ttu-id="bf2cf-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="bf2cf-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bf2cf-113">Če imate težave z zagonom storitve, zaženite ta ukaz tako, da odprete ukazni poziv s povišanimi dovoljenji:</span><span class="sxs-lookup"><span data-stu-id="bf2cf-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bf2cf-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="bf2cf-114">**sfc /scannow**</span></span>

<span data-ttu-id="bf2cf-115">Ko se ukaz konča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="bf2cf-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bf2cf-116">Če želite podrobnejše informacije, glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Ko aktivirate Office v storitvi Microsoft 365, poskusite znova» napaka «](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bf2cf-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>