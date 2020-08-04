---
title: Uporaba skupine TeamViewer za oddaljeno skrbništvo naprav Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555750"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="a7776-102">Uporaba skupine TeamViewer za oddaljeno skrbništvo naprav Intune</span><span class="sxs-lookup"><span data-stu-id="a7776-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="a7776-103">Naprave, ki jih upravlja Intune, se lahko upravljajo na daljavo z [uporabo TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="a7776-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="a7776-104">Če želite upravljati Intune s funkcijo TeamViewer, uporabite te korake:</span><span class="sxs-lookup"><span data-stu-id="a7776-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="a7776-105">Začnite s pridobivanjem poverilnic iz TeamViewer za nastavitev TeamViewer Connector na Intune.</span><span class="sxs-lookup"><span data-stu-id="a7776-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="a7776-106">To omogoča admin, da vnesete poverilnice v TeamViewer Connector UI pod Naprave, enkratna operacija za vzpostavitev povezave med Intune in TeamViewer storitev.</span><span class="sxs-lookup"><span data-stu-id="a7776-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="a7776-107">**1. del: začetek seje z oddaljeno napravo**</span><span class="sxs-lookup"><span data-stu-id="a7776-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="a7776-108">V **razdelku Vse**naprave izberite napravo, s katerim želite začeti oddaljeno sejo.</span><span class="sxs-lookup"><span data-stu-id="a7776-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="a7776-109">Iz **... Več**, izberite **Nova seja oddaljene pomoči**.</span><span class="sxs-lookup"><span data-stu-id="a7776-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="a7776-110">Izberite **Da,** če želite potrditi, da želite vzpostaviti oddaljeno sejo.</span><span class="sxs-lookup"><span data-stu-id="a7776-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="a7776-111">Ko storitev TeamViewer priznava zahtevo »Začetek nove oddaljene seje«, boste videli možnost **zagona oddaljene pomoči** pod podrobnostmi podokna »Pregled«ali »Essentials«) za napravo.</span><span class="sxs-lookup"><span data-stu-id="a7776-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="a7776-112">Izberite **Kliknite več,** če želite razširiti podokno in prikazati stanje oddaljene pomoči.</span><span class="sxs-lookup"><span data-stu-id="a7776-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="a7776-113">Izberite **Zaženi oddaljeno** sejo, da sprožite sejo na skrbniški strani.</span><span class="sxs-lookup"><span data-stu-id="a7776-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="a7776-114">Izberite, ali želite prenesti binarno datoteko TeamViewer (Windows), in izberite **Zaženi**.</span><span class="sxs-lookup"><span data-stu-id="a7776-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="a7776-115">\*\* Opomba\*\* Prezrete lahko katero koli stran spletnega brskalnika, ki je odprta na spletnem mestu TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="a7776-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="a7776-116">Potrdite zahtevo, da program TeamViewer spremeni napravo (samo windows).</span><span class="sxs-lookup"><span data-stu-id="a7776-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="a7776-117">Program TeamViewer se zažene in vključuje kodo seje za preverjanje pristnosti povezave z oddaljeno napravo.</span><span class="sxs-lookup"><span data-stu-id="a7776-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="a7776-118">**Del 2: Na napravi, ki je usmerjena v oddaljeno sejo**</span><span class="sxs-lookup"><span data-stu-id="a7776-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="a7776-119">Odprite portal podjetja Intune.</span><span class="sxs-lookup"><span data-stu-id="a7776-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="a7776-120">Poiščite zastavico obvestila: »Skrbnik za IT zahteva nadzor nad to napravo za sejo oddaljene pomoči« in izberite obvestilo.</span><span class="sxs-lookup"><span data-stu-id="a7776-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="a7776-121">Izberite prenos aplikacije TeamViewer ali potrdite prenos aplikacije TeamViewer iz trgovine z aplikacijami in izberite **Zaženi**.</span><span class="sxs-lookup"><span data-stu-id="a7776-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="a7776-122">\*\* Opomba\*\* Prezrete lahko katero koli stran spletnega brskalnika, ki je odprta na spletnem mestu TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="a7776-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="a7776-123">Potrdite zahtevo, da program TeamViewer spremeni napravo (samo windows).</span><span class="sxs-lookup"><span data-stu-id="a7776-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="a7776-124">Program TeamViewer se zažene in vključuje kodo seje za preverjanje pristnosti povezave z oddaljeno napravo.</span><span class="sxs-lookup"><span data-stu-id="a7776-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="a7776-125">Pojavno okno vas vpraša, ali želite dovoliti začetek seje.</span><span class="sxs-lookup"><span data-stu-id="a7776-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="a7776-126">\*\* Opomba\*\* Kode sej, ki jih ustvari storitev TeamViewer, so samo enkratne uporabe.</span><span class="sxs-lookup"><span data-stu-id="a7776-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="a7776-127">Če izgubite povezavo, morate:</span><span class="sxs-lookup"><span data-stu-id="a7776-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="a7776-128">Zaprite primerek aplikacije TeamViewer v oddaljeni napravi in skrbniški delovni postaji.</span><span class="sxs-lookup"><span data-stu-id="a7776-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="a7776-129">Zaprite portal podjetja v oddaljeni napravi.</span><span class="sxs-lookup"><span data-stu-id="a7776-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="a7776-130">Začnite novo »novo sejo oddaljene pomoči« iz skrbniškega portala.</span><span class="sxs-lookup"><span data-stu-id="a7776-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="a7776-131">Skozi okno portal podjetja v oddaljeni napravi uprite, da prejmete novo obvestilo.</span><span class="sxs-lookup"><span data-stu-id="a7776-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="a7776-132">Prenesite in odprite aplikacijo TeamViewer v oddaljeni napravi in skrbniški delovni postaji, kot prej.</span><span class="sxs-lookup"><span data-stu-id="a7776-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>