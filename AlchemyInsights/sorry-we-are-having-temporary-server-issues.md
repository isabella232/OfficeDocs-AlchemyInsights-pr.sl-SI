---
title: Pritrjevanje aplikacij za Microsoft 365 Žal mi je, da imamo začasno sporočilo o težavah strežnika
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582719"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="99a7b-102">Pritrjevanje Microsoft 365 apps "Oprostite, imamo začasna vprašanja strežnika" sporočilo</span><span class="sxs-lookup"><span data-stu-id="99a7b-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="99a7b-103">Če prejmete to sporočilo, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="99a7b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="99a7b-104">Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Microsoftovih aplikacij za 365.</span><span class="sxs-lookup"><span data-stu-id="99a7b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="99a7b-105">Glejte [URL-je in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="99a7b-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="99a7b-106">Iti k **začetek**  >  **prost dostop**, ter torej stavek **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="99a7b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="99a7b-107">Zagotovite, da se izvajajo naslednje storitve:</span><span class="sxs-lookup"><span data-stu-id="99a7b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="99a7b-108">Samodejna nastavitev omrežne priključene naprave</span><span class="sxs-lookup"><span data-stu-id="99a7b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="99a7b-109">Storitev omrežnega seznama</span><span class="sxs-lookup"><span data-stu-id="99a7b-109">Network List Service</span></span>
    - <span data-ttu-id="99a7b-110">Omrežna lokacija zavedanje</span><span class="sxs-lookup"><span data-stu-id="99a7b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="99a7b-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="99a7b-111">Windows Event Log</span></span>

<span data-ttu-id="99a7b-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="99a7b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="99a7b-113">Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:</span><span class="sxs-lookup"><span data-stu-id="99a7b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="99a7b-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="99a7b-114">**sfc /scannow**</span></span>

<span data-ttu-id="99a7b-115">Ko se ta ukaz dokonča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="99a7b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="99a7b-116">Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "Napaka pri aktiviranju](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="99a7b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>