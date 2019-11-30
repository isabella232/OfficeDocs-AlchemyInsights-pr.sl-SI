---
title: Activation Issue-ne moremo povezati prav zdaj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628258"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="1b34f-102">Popravljanje Officeovih aplikacij» trenutno ne moremo vzpostaviti sporočila «</span><span class="sxs-lookup"><span data-stu-id="1b34f-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="1b34f-103">Če prejmete to sporočilo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="1b34f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1b34f-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Officeovih aplikacij.</span><span class="sxs-lookup"><span data-stu-id="1b34f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="1b34f-105">Glejte [URL-je sistema Office 365 in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1b34f-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="1b34f-106">Iti k **začetek** > **prost dostop**, ter torej stavek **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="1b34f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="1b34f-107">Zagotovite, da se izvajajo naslednje storitve:</span><span class="sxs-lookup"><span data-stu-id="1b34f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="1b34f-108">Samodejna nastavitev omrežne priključene naprave</span><span class="sxs-lookup"><span data-stu-id="1b34f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="1b34f-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="1b34f-109">Network List Service</span></span>
    - <span data-ttu-id="1b34f-110">Omrežna lokacija zavedanje</span><span class="sxs-lookup"><span data-stu-id="1b34f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="1b34f-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="1b34f-111">Windows Event Log</span></span>

<span data-ttu-id="1b34f-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="1b34f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="1b34f-113">Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:</span><span class="sxs-lookup"><span data-stu-id="1b34f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="1b34f-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="1b34f-114">**sfc /scannow**</span></span>

<span data-ttu-id="1b34f-115">Ko se ta ukaz dokonča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="1b34f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="1b34f-116">Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "napako, ko aktivirate Office iz Officea 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="1b34f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>