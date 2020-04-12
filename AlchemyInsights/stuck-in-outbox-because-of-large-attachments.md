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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232646"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="410ab-102">Popravljanje sporočil, ki so obtičala v mapi» Odpošlji «</span><span class="sxs-lookup"><span data-stu-id="410ab-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="410ab-103">Priporočamo, da začnete tako, da zaženete scenarij [» Imam težave pri pošiljanju, prejemanju ali iskanju e-poštnih sporočil «](https://aka.ms/SaRA-OutlookSendReceive) iz [Microsoftovega orodja za podporo in obnovitev](https://diagnostics.office.com/#/) v prizadetem računalniku.</span><span class="sxs-lookup"><span data-stu-id="410ab-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="410ab-104">Ko se sporočilo zatakne v mapi» Odpošlji «, je najverjetnejši vzrok velika pripona ali možnost» Pošlji takoj, ko je vzpostavljena povezava «ni omogočena.</span><span class="sxs-lookup"><span data-stu-id="410ab-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="410ab-105">**Odstranjevanje velike pritrditve**</span><span class="sxs-lookup"><span data-stu-id="410ab-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="410ab-106">Kliknite **Pošlji/Prejmi** > **delo brez povezave**.</span><span class="sxs-lookup"><span data-stu-id="410ab-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="410ab-107">V podoknu za krmarjenje kliknite **Odpošlji**.</span><span class="sxs-lookup"><span data-stu-id="410ab-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="410ab-108">Od tu lahko:</span><span class="sxs-lookup"><span data-stu-id="410ab-108">From here, you can:</span></span> 
    - <span data-ttu-id="410ab-109">Izbrišite sporočilo.</span><span class="sxs-lookup"><span data-stu-id="410ab-109">Delete the message.</span></span> <span data-ttu-id="410ab-110">Šele izbrati to ter udarjanje z nogo ob nogo **izbrisati**.</span><span class="sxs-lookup"><span data-stu-id="410ab-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="410ab-111">Povlecite sporočilo v **mapo Osnutki**, dvokliknite, da odprete sporočilo, in izbrišite Prilogo (kliknite nanj in kliknite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="410ab-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="410ab-112">Če napaka pove, da Outlook poskuša posredovati sporočilo, zaprite Outlook.</span><span class="sxs-lookup"><span data-stu-id="410ab-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="410ab-113">Lahko traja nekaj trenutkov za izhod.</span><span class="sxs-lookup"><span data-stu-id="410ab-113">It may take a few moments to exit.</span></span> <span data-ttu-id="410ab-114">Če se Outlook ne zapre, pritisnite **CTRL + ALT + DELETE** in kliknite **Zaženi upravitelja opravil**.</span><span class="sxs-lookup"><span data-stu-id="410ab-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="410ab-115">V upravitelju opravil izberite zavihek **procesi** , se pomaknite navzdol do možnosti Outlook. exe in kliknite **Končaj proces**.</span><span class="sxs-lookup"><span data-stu-id="410ab-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="410ab-116">Ko se Outlook zapre, znova zaženite Outlook in ponovite korake 2-3.</span><span class="sxs-lookup"><span data-stu-id="410ab-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="410ab-117">Ko odstranite Prilogo, kliknite **Pošlji/Prejmi** > **delo brez povezave** , da počistite gumb in nadaljujete delo v spletu.</span><span class="sxs-lookup"><span data-stu-id="410ab-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="410ab-118">Sporočila se tudi zataknejo v mapi» **Odpošlji**«, ko kliknete Pošlji, vendar niste povezani.</span><span class="sxs-lookup"><span data-stu-id="410ab-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="410ab-119">Kliknite **Pošlji/Prejmi** in si oglejte **delovni gumb brez povezave** .</span><span class="sxs-lookup"><span data-stu-id="410ab-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="410ab-120">Če je modra, si izključen.</span><span class="sxs-lookup"><span data-stu-id="410ab-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="410ab-121">Kliknite na povezavo (gumb se obarva belo) in kliknite **Pošlji vse**.</span><span class="sxs-lookup"><span data-stu-id="410ab-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="410ab-122">**Omogoči pošiljanje takoj, ko je priključen**</span><span class="sxs-lookup"><span data-stu-id="410ab-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="410ab-123">Na kartici Datoteka kliknite **možnosti**.</span><span class="sxs-lookup"><span data-stu-id="410ab-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="410ab-124">V pogovornem oknu možnosti programa Outlook kliknite **Napredno**.</span><span class="sxs-lookup"><span data-stu-id="410ab-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="410ab-125">V odseku Pošlji in prejmi kliknite, če želite omogočiti **pošiljanje takoj, ko je priključen**.</span><span class="sxs-lookup"><span data-stu-id="410ab-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="410ab-126">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="410ab-126">Click **OK**.</span></span>
 
<span data-ttu-id="410ab-127">Za vse podrobnosti glejte:</span><span class="sxs-lookup"><span data-stu-id="410ab-127">For full details, see:</span></span>
- [<span data-ttu-id="410ab-128">Videoposnetek: pošiljanje ali brisanje zagozdila e-poštnega sporočila</span><span class="sxs-lookup"><span data-stu-id="410ab-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="410ab-129">E-pošta ostane v mapi» Odpošlji «, dokler ročno ne sprožite operacije pošiljanja/prejemanja v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="410ab-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
