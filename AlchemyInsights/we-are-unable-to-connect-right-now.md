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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581891"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="1254d-102">Pritrjevanje Microsoft 365 apps "mi se ne more povezati zdaj" sporočilo</span><span class="sxs-lookup"><span data-stu-id="1254d-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="1254d-103">Če prejmete to sporočilo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="1254d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1254d-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Microsoftovih aplikacij za 365.</span><span class="sxs-lookup"><span data-stu-id="1254d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="1254d-105">Glejte [Microsoft URL-ji in obsegi naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1254d-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="1254d-106">Iti k **začetek**  >  **prost dostop**, ter torej stavek **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="1254d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="1254d-107">Zagotovite, da se izvajajo naslednje storitve:</span><span class="sxs-lookup"><span data-stu-id="1254d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="1254d-108">Samodejna nastavitev omrežne priključene naprave</span><span class="sxs-lookup"><span data-stu-id="1254d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="1254d-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="1254d-109">Network List Service</span></span>
    - <span data-ttu-id="1254d-110">Omrežna lokacija zavedanje</span><span class="sxs-lookup"><span data-stu-id="1254d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="1254d-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="1254d-111">Windows Event Log</span></span>

<span data-ttu-id="1254d-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="1254d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="1254d-113">Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:</span><span class="sxs-lookup"><span data-stu-id="1254d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="1254d-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="1254d-114">**sfc /scannow**</span></span>

<span data-ttu-id="1254d-115">Ko se ta ukaz dokonča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="1254d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="1254d-116">Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "napako, ko aktivirate Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="1254d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>