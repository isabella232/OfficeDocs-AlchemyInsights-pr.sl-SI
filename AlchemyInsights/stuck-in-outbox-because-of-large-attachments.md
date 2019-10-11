---
title: Zaljubljen v odpošiljanju zaradi velikih prilog
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441321"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="858c6-102">Popravljanje sporočil, ki so obtičala v mapi» Odpošlji «</span><span class="sxs-lookup"><span data-stu-id="858c6-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="858c6-103">Priporočamo, da začnete tako, da zaženete scenarij [» Imam težave pri pošiljanju, prejemanju ali iskanju e-poštnih sporočil «](https://aka.ms/SaRA-OutlookSendReceive) iz [Microsoftovega orodja za podporo in obnovitev](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="858c6-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="858c6-104">Ko se sporočilo v mapi» Odpošlji «ujame, so najverjetnejši vzroki:</span><span class="sxs-lookup"><span data-stu-id="858c6-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="858c6-105">Velike priponke.</span><span class="sxs-lookup"><span data-stu-id="858c6-105">Large attachments.</span></span>
- <span data-ttu-id="858c6-106">**Pošlji takoj, ko je povezana** možnost ni omogočena.</span><span class="sxs-lookup"><span data-stu-id="858c6-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="858c6-107">Če želite odstraniti velike Priloge:</span><span class="sxs-lookup"><span data-stu-id="858c6-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="858c6-108">V Outlooku izberite **Pošlji/Prejmi** > **delo brez povezave**.</span><span class="sxs-lookup"><span data-stu-id="858c6-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="858c6-109">V podoknu za krmarjenje izberite **Odpošlji**.</span><span class="sxs-lookup"><span data-stu-id="858c6-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="858c6-110">Od tu lahko:</span><span class="sxs-lookup"><span data-stu-id="858c6-110">From here, you can:</span></span> 
    - <span data-ttu-id="858c6-111">Izbrišite sporočilo (izberite ga in izberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="858c6-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="858c6-112">Povlecite sporočilo v mapo Osnutki, dvokliknite, da ga odprete, in odstranite Prilogo in izberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="858c6-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="858c6-113">Če se prikaže napaka, ki pravi, da Outlook poskuša posredovati sporočilo, zaprite Outlook.</span><span class="sxs-lookup"><span data-stu-id="858c6-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="858c6-114">Lahko traja nekaj trenutkov za izhod.</span><span class="sxs-lookup"><span data-stu-id="858c6-114">It may take a few moments to exit.</span></span> <span data-ttu-id="858c6-115">Če se Outlook ne zapre, pritisnite CTRL + ALT + DELETE in izberite **Zaženi upravitelja opravil**.</span><span class="sxs-lookup"><span data-stu-id="858c6-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="858c6-116">V upravitelju opravil izberite zavihek **procesi** , se pomaknite navzdol do možnosti Outlook. exe in izberite **Končaj proces**.</span><span class="sxs-lookup"><span data-stu-id="858c6-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="858c6-117">Ko se Outlook zapre, ga znova zaženite in ponovite korake 2 in 3.</span><span class="sxs-lookup"><span data-stu-id="858c6-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="858c6-118">Ko odstranite Prilogo, kliknite **Pošlji/Prejmi** > **delo brez povezave** , da nadaljujete delo v spletu.</span><span class="sxs-lookup"><span data-stu-id="858c6-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="858c6-119">Sporočila se tudi zataknejo v mapi» **Odpošlji**«, ko kliknete Pošlji, vendar niste povezani.</span><span class="sxs-lookup"><span data-stu-id="858c6-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="858c6-120">Kliknite **Pošlji/Prejmi** in si oglejte **delovni gumb brez povezave** .</span><span class="sxs-lookup"><span data-stu-id="858c6-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="858c6-121">Če je modra, si izključen.</span><span class="sxs-lookup"><span data-stu-id="858c6-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="858c6-122">Izberite jo za povezavo (gumb se obarva belo) in kliknite **Pošlji vse**.</span><span class="sxs-lookup"><span data-stu-id="858c6-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="858c6-123">Če želite omogočiti **pošiljanje takoj, ko je priključen**:</span><span class="sxs-lookup"><span data-stu-id="858c6-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="858c6-124">Izberite \*\*\*\* > \*\*\*\* možnosti >  datoteke**Napredno**.</span><span class="sxs-lookup"><span data-stu-id="858c6-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="858c6-125">V odseku **Pošlji in prejmi** izberite **Pošlji takoj, ko je povezava vzpostavljena**, nato pa izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="858c6-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="858c6-126">Za podrobnejše informacije glej:</span><span class="sxs-lookup"><span data-stu-id="858c6-126">For full details see:</span></span>
- [<span data-ttu-id="858c6-127">Videoposnetek: pošiljanje ali brisanje zagozdila e-poštnega sporočila</span><span class="sxs-lookup"><span data-stu-id="858c6-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="858c6-128">E-pošta ostane v mapi» Odpošlji «, dokler ročno ne sprožite operacije pošiljanja/prejemanja v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="858c6-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
