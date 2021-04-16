---
title: Težava z aktiviranjem – trenutno ni mogoče vzpostaviti povezave
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806458"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="43b77-102">Popravljanje sporočil »Trenutno ni mogoče vzpostaviti povezave« v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="43b77-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="43b77-103">Če se prikaže to sporočilo, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="43b77-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="43b77-104">Preverite nastavitve požarnega zidu, protivirusne programske opreme in strežnika proxy, da potrdite, da ne blokirajo dostopa do interneta do aplikacij storitve Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="43b77-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="43b77-105">Glejte [Microsoftovi URL-ji in obsegi naslovov IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="43b77-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="43b77-106">Odprite začetni **meni**  >  **Zaženi** in vnesite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="43b77-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="43b77-107">Prepričajte se, da so vse te storitve zagnane:</span><span class="sxs-lookup"><span data-stu-id="43b77-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="43b77-108">Samodejna nastavitev naprav, povezanih z omrežjem</span><span class="sxs-lookup"><span data-stu-id="43b77-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="43b77-109">Omrežna storitev seznama</span><span class="sxs-lookup"><span data-stu-id="43b77-109">Network List Service</span></span>
    - <span data-ttu-id="43b77-110">Ozaveščenost o omrežnem mestu</span><span class="sxs-lookup"><span data-stu-id="43b77-110">Network Location Awareness</span></span>
    - <span data-ttu-id="43b77-111">Dnevnik dogodkov sistema Windows</span><span class="sxs-lookup"><span data-stu-id="43b77-111">Windows Event Log</span></span>

<span data-ttu-id="43b77-112">Če se ena od teh storitev ne izvaja, jo poskusite zagnati.</span><span class="sxs-lookup"><span data-stu-id="43b77-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="43b77-113">Če imate težave pri zagonu storitve, zaženite ta ukaz tako, da odprete ukazni poziv z povečanimi dovoljenji:</span><span class="sxs-lookup"><span data-stu-id="43b77-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="43b77-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="43b77-114">**sfc /scannow**</span></span>

<span data-ttu-id="43b77-115">Ko se ta ukaz dokonča, znova zaženite računalnik.</span><span class="sxs-lookup"><span data-stu-id="43b77-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="43b77-116">Če želite podrobne informacije, glejte [»Povezave z vašim računom žal ni mogoče vzpostaviti. Pri aktiviranju Officea v storitvi Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)se prikaže sporočilo o napaki »Poskusite znova pozneje«.</span><span class="sxs-lookup"><span data-stu-id="43b77-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>