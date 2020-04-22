---
title: Pritrjevanje Officeovih aplikacij Žal mi je, da imamo sporočilo o začasnih težavah s strežnikom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764133"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="51bbe-102">Popravljanje Officeovih aplikacij» Žal mi je, da imamo sporočilo o začasnih težavah v strežniku «</span><span class="sxs-lookup"><span data-stu-id="51bbe-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="51bbe-103">Če prejmete to sporočilo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="51bbe-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="51bbe-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Officeovih aplikacij.</span><span class="sxs-lookup"><span data-stu-id="51bbe-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="51bbe-105">Glejte [URL-je in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="51bbe-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="51bbe-106">Iti k **začetek** > **prost dostop**, ter torej stavek **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="51bbe-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="51bbe-107">Zagotovite, da se izvajajo naslednje storitve:</span><span class="sxs-lookup"><span data-stu-id="51bbe-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="51bbe-108">Samodejna nastavitev omrežne priključene naprave</span><span class="sxs-lookup"><span data-stu-id="51bbe-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="51bbe-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="51bbe-109">Network List Service</span></span>
    - <span data-ttu-id="51bbe-110">Omrežna lokacija zavedanje</span><span class="sxs-lookup"><span data-stu-id="51bbe-110">Network Location Awareness</span></span>
    - <span data-ttu-id="51bbe-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="51bbe-111">Windows Event Log</span></span>

<span data-ttu-id="51bbe-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="51bbe-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="51bbe-113">Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:</span><span class="sxs-lookup"><span data-stu-id="51bbe-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="51bbe-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="51bbe-114">**sfc /scannow**</span></span>

<span data-ttu-id="51bbe-115">Ko se ta ukaz dokonča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="51bbe-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="51bbe-116">Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "Napaka pri aktiviranju](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="51bbe-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>