---
title: Odpravljanje težav s programom Microsoft 365 žal imamo sporočilo o začasnih težavah s strežnikom
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758261"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="94e42-102">Odpravljanje težav s storitvijo Microsoft 365» žal imamo sporočilo o začasnih težavah s strežnikom «</span><span class="sxs-lookup"><span data-stu-id="94e42-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="94e42-103">Če prejmete to sporočilo, naredite to:</span><span class="sxs-lookup"><span data-stu-id="94e42-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="94e42-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve strežnika proxy, da potrdite, da ne blokirajo internetnega dostopa do programov Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="94e42-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="94e42-105">Prikaz [URL-jev in obsegov naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="94e42-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="94e42-106">Pojdite na **začetek**  >  **Zaženi**in vnesite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="94e42-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="94e42-107">Zagotovite, da se izvajajo te storitve:</span><span class="sxs-lookup"><span data-stu-id="94e42-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="94e42-108">Samodejna nastavitev omrežnih naprav, povezanih z omrežjem</span><span class="sxs-lookup"><span data-stu-id="94e42-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="94e42-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="94e42-109">Network List Service</span></span>
    - <span data-ttu-id="94e42-110">Poznavanje omrežnega mesta</span><span class="sxs-lookup"><span data-stu-id="94e42-110">Network Location Awareness</span></span>
    - <span data-ttu-id="94e42-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="94e42-111">Windows Event Log</span></span>

<span data-ttu-id="94e42-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="94e42-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="94e42-113">Če imate težave z zagonom storitve, zaženite ta ukaz tako, da odprete ukazni poziv s povišanimi dovoljenji:</span><span class="sxs-lookup"><span data-stu-id="94e42-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="94e42-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="94e42-114">**sfc /scannow**</span></span>

<span data-ttu-id="94e42-115">Ko se ukaz konča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="94e42-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="94e42-116">Če želite podrobnejše informacije, glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Ko aktivirate sporočilo o napaki, poskusite znova](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="94e42-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>