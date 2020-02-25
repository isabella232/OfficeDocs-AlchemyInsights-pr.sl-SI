---
title: Odpravljanje težav z Bluetoothom v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268709"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="eb537-102">Odpravljanje težav z Bluetoothom v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="eb537-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="eb537-103">Če ikona Bluetooth manjka ali Bluetooth ni mogoče vklopiti ali izklopiti, boste morda želeli zagnati orodje za odpravljanje težav s tehnologijo Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="eb537-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="eb537-104">[Odprite nastavitve za odpravljanje težav](ms-settings:troubleshoot), kliknite **Bluetooth** pod **Poišči in odpravite druge težave**, kliknite **Zaženi orodje za odpravljanje težav**.</span><span class="sxs-lookup"><span data-stu-id="eb537-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="eb537-105">Če ne vidite ikone Bluetooth, vendar se Bluetooth pojavlja v upravitelju naprav:</span><span class="sxs-lookup"><span data-stu-id="eb537-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="eb537-106">V upravitelju naprav kliknite **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="eb537-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="eb537-107">Pritisnite in pridržite (ali z desno tipko miške kliknite) ime adapterja Bluetooth in kliknite **Odstrani napravo**.</span><span class="sxs-lookup"><span data-stu-id="eb537-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="eb537-108">Zaustavite napravo s sistemom Windows, počakajte nekaj sekund in jo znova vklopite.</span><span class="sxs-lookup"><span data-stu-id="eb537-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="eb537-109">Windows bo poskusil znova namestiti gonilnik.</span><span class="sxs-lookup"><span data-stu-id="eb537-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="eb537-110">Če ste pred kratkim namestili posodobitve sistema Windows 10 ali nadgradili na Windows 10, boste morda želeli preveriti, ali so na voljo posodobitve gonilnikov:</span><span class="sxs-lookup"><span data-stu-id="eb537-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="eb537-111">V upravitelju naprav kliknite **Bluetooth**in nato še ime adapterja Bluetooth (ki lahko vključuje besedo» radio «).</span><span class="sxs-lookup"><span data-stu-id="eb537-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="eb537-112">Pritisnite in pridržite (ali z desno tipko miške kliknite) adapter Bluetooth, nato pa kliknite **Posodobi** > **samodejno iskanje gonilnika za posodobljeno programsko opremo gonilnika**.</span><span class="sxs-lookup"><span data-stu-id="eb537-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="eb537-113">Sledite korakom in kliknite **Zapri**.</span><span class="sxs-lookup"><span data-stu-id="eb537-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="eb537-114">Če Windows ne najde novega gonilnika Bluetooth, obiščite spletno mesto izdelovalca računalnika in prenesite najnovejši gonilnik Bluetooth od tam.</span><span class="sxs-lookup"><span data-stu-id="eb537-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="eb537-115">Ko jo prenesete, kliknite **Posodobi gonilnik** > **brskanje po mojem računalniku za programsko opremo** > gonilnika**poiščite** mesto, kjer so shranjene datoteke gonilnika > **OK** > **Next**in sledite navodilom za namestitev.</span><span class="sxs-lookup"><span data-stu-id="eb537-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="eb537-116">Po namestitvi posodobljenega gonilnika znova zaženite računalnik in preverite, ali to odpravlja težavo s povezavo.</span><span class="sxs-lookup"><span data-stu-id="eb537-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="eb537-117">Če želite več podrobnosti o odpravljanju težav z Bluetoothom, si oglejte celoten članek, [odpravite težave s tehnologijo Bluetooth v sistemu Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="eb537-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
