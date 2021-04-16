---
title: Manjkajoči ikoni »Napajanje« ali »Baterija« v Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790564"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="2908b-102">Manjkajoči ikoni »Napajanje« ali »Baterija« v Windows 10</span><span class="sxs-lookup"><span data-stu-id="2908b-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="2908b-103">Če ima vaša naprava s sistemom Windows 10 baterijo (npr. prenosnik ali tablični računalnik ali osebni računalnik, povezan z UPS-jem prek USB-ja), je v opravilni vrstici blizu ure ponavadi prikazana ikona napajanja/baterije, na primer:</span><span class="sxs-lookup"><span data-stu-id="2908b-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona »Baterija«](media/battery-icon.png)

<span data-ttu-id="2908b-105">Če ikone ne vidite, je morda skrita:</span><span class="sxs-lookup"><span data-stu-id="2908b-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="2908b-106">Pojdite na **[Nastavitve > Prilagajanje > Opravilna vrstica](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="2908b-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="2908b-107">V območju za obvestila kliknite **Izberite, katere ikone naj se prikažejo v opravilni vrstici**.</span><span class="sxs-lookup"><span data-stu-id="2908b-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="2908b-108">Nato na seznamu poiščite element **Napajanje** in njegovo nastavitev preklopite na **Vklopljeno**.</span><span class="sxs-lookup"><span data-stu-id="2908b-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Prikažite ikono »Napajanje« v opravilni vrstici](media/power-icon-on.png)

<span data-ttu-id="2908b-110">**Odpravljanje težav**</span><span class="sxs-lookup"><span data-stu-id="2908b-110">**Troubleshooting**</span></span>

<span data-ttu-id="2908b-111">Če ste sledili zgornjim navodilom in je preklopni gumb **Napajanje** zatemnjen ali ni viden, v iskalno polje v opravilni vrstici vnesite **upravitelj naprav**, in na seznamu rezultatov izberite **Upravitelj naprav**.</span><span class="sxs-lookup"><span data-stu-id="2908b-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="2908b-112">V razdelku **Baterije**, z desno tipko miške kliknite baterijo za svojo napravo **Onemogoči** in kliknite **Da**.</span><span class="sxs-lookup"><span data-stu-id="2908b-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="2908b-113">Počakajte nekaj sekund, nato z desno tipko miške kliknite baterijo in kliknite **Omogoči**.</span><span class="sxs-lookup"><span data-stu-id="2908b-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="2908b-114">Znova zaženite napravo.</span><span class="sxs-lookup"><span data-stu-id="2908b-114">Then restart your device.</span></span>

<span data-ttu-id="2908b-115">Če ste sledili zgornjim navodilom, vendar se ikona akumulatorja ne prikaže v opravilni vrstici, v iskalno polje v opravilni vrstici vtipkajte **upravitelj opravil** in na seznamu rezultatov kliknite **Upravitelj opravil**.</span><span class="sxs-lookup"><span data-stu-id="2908b-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="2908b-116">Na zavihku **Postopki** pod **Ime** z desno tipko miške kliknite **Raziskovalec** in nato **Ponovni zagon**.</span><span class="sxs-lookup"><span data-stu-id="2908b-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
