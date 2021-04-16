---
title: Odpravljanje težav z vmesnikom Bluetooth v sistemu Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812948"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="7d879-102">Odpravljanje težav z vmesnikom Bluetooth v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="7d879-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="7d879-103">Če manjka ikona za Bluetooth ali pa povezave Bluetooth ni mogoče vklopite ali izklopiti, zaženite orodje za odpravljanje težav s povezavo Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="7d879-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="7d879-104">[Odprite nastavitve za odpravljanje težav](ms-settings:troubleshoot), kliknite **Bluetooth** v razdelku Iskanje in odpravljanje **drugih težav**, nato pa **kliknite Zaženi orodje za odpravljanje težav.**</span><span class="sxs-lookup"><span data-stu-id="7d879-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="7d879-105">Če ikone za Bluetooth ne vidite, vendar je Bluetooth prikazan v upravitelju naprav:</span><span class="sxs-lookup"><span data-stu-id="7d879-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="7d879-106">V upravitelju naprav kliknite **Bluetooth.**</span><span class="sxs-lookup"><span data-stu-id="7d879-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="7d879-107">Pritisnite in pridržite (ali z desno tipko miške kliknite) ime vmesnika Bluetooth in kliknite **Odstrani napravo.**</span><span class="sxs-lookup"><span data-stu-id="7d879-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="7d879-108">Zaustavite napravo s sistemom Windows, počakajte nekaj sekund, nato pa jo znova vklopite.</span><span class="sxs-lookup"><span data-stu-id="7d879-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="7d879-109">Windows bo poskusil znova namestiti gonilnik.</span><span class="sxs-lookup"><span data-stu-id="7d879-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="7d879-110">Če ste nedavno namestili posodobitve sistema Windows 10 ali nadgradili na Windows 10, boste morda želeli preveriti, ali so na voljo posodobitve gonilnikov:</span><span class="sxs-lookup"><span data-stu-id="7d879-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="7d879-111">V upravitelju naprav kliknite **Bluetooth**, nato pa kliknite ime vmesnika Bluetooth (ki lahko vključuje besedo »radio«).</span><span class="sxs-lookup"><span data-stu-id="7d879-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="7d879-112">Pritisnite in pridržite (ali z desno tipko miške kliknite) vmesnik Bluetooth, nato pa kliknite Samodejno posodobi **gonilnik** Poišči  >  **posodobljeno programsko opremo gonilnika**.</span><span class="sxs-lookup"><span data-stu-id="7d879-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="7d879-113">Upoštevajte navodila, nato pa kliknite **Zapri.**</span><span class="sxs-lookup"><span data-stu-id="7d879-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="7d879-114">Če Sistem Windows ne najde novega gonilnika Za Bluetooth, obiščite spletno mesto izdelovalca računalnika in prenesite najnovejši gonilnik za Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="7d879-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="7d879-115">Ko ga prenesete, kliknite Posodobi gonilnik Poišči programsko opremo v mojem računalniku Poiščite mesto, kjer so shranjene datoteke gonilnika > V redu Naprej > sledite navodilom  >    >     >  za namestitev.</span><span class="sxs-lookup"><span data-stu-id="7d879-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="7d879-116">Po namestitvi posodobljenega gonilnika znova zaženite računalnik in nato preverite, ali s tem odpravite težavo s povezavo.</span><span class="sxs-lookup"><span data-stu-id="7d879-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="7d879-117">Če želite več informacij o odpravljanju težav z vmesnikom Bluetooth, preberite celoten članek Odpravljanje težav [z vmesnikom Bluetooth v sistemu Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="7d879-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
