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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716188"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="d9cc0-102">Popravljanje Officeovih aplikacij» trenutno ne moremo vzpostaviti sporočila «</span><span class="sxs-lookup"><span data-stu-id="d9cc0-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="d9cc0-103">Če prejmete to sporočilo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="d9cc0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d9cc0-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Officeovih aplikacij.</span><span class="sxs-lookup"><span data-stu-id="d9cc0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="d9cc0-105">Glejte [Microsoft URL-ji in obsegi naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d9cc0-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d9cc0-106">Iti k **začetek** > **prost dostop**, ter torej stavek **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="d9cc0-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d9cc0-107">Zagotovite, da se izvajajo naslednje storitve:</span><span class="sxs-lookup"><span data-stu-id="d9cc0-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d9cc0-108">Samodejna nastavitev omrežne priključene naprave</span><span class="sxs-lookup"><span data-stu-id="d9cc0-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d9cc0-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="d9cc0-109">Network List Service</span></span>
    - <span data-ttu-id="d9cc0-110">Omrežna lokacija zavedanje</span><span class="sxs-lookup"><span data-stu-id="d9cc0-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d9cc0-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="d9cc0-111">Windows Event Log</span></span>

<span data-ttu-id="d9cc0-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="d9cc0-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d9cc0-113">Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:</span><span class="sxs-lookup"><span data-stu-id="d9cc0-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d9cc0-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="d9cc0-114">**sfc /scannow**</span></span>

<span data-ttu-id="d9cc0-115">Ko se ta ukaz dokonča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="d9cc0-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d9cc0-116">Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "napako, ko aktivirate Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="d9cc0-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>