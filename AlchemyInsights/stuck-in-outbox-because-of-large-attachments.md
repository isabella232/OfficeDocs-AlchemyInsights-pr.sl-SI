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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241268"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="edd9a-102">Popravljanje sporočil, ki so obtičala v mapi» Odpošlji «</span><span class="sxs-lookup"><span data-stu-id="edd9a-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="edd9a-103">Priporočamo, da začnete tako, da zaženete scenarij [» Imam težave pri pošiljanju, prejemanju ali iskanju e-poštnih sporočil «](https://aka.ms/SaRA-OutlookSendReceive) iz [Microsoftovega orodja za podporo in obnovitev](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="edd9a-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="edd9a-104">Ko se sporočilo zatakne v mapi» Odpošlji «, je najverjetnejši vzrok velika pripona ali možnost» Pošlji takoj, ko je vzpostavljena povezava «ni omogočena.</span><span class="sxs-lookup"><span data-stu-id="edd9a-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="edd9a-105">**Odstranjevanje velike pritrditve**</span><span class="sxs-lookup"><span data-stu-id="edd9a-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="edd9a-106">V Outlooku izberite **Pošlji/Prejmi** > **delo brez povezave**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="edd9a-107">V podoknu za krmarjenje izberite **Odpošlji**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="edd9a-108">Od tu lahko:</span><span class="sxs-lookup"><span data-stu-id="edd9a-108">From here, you can:</span></span> 
    - <span data-ttu-id="edd9a-109">Izbrišite sporočilo (izberite ga in izberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="edd9a-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="edd9a-110">Povlecite sporočilo v mapo Osnutki, dvokliknite, da ga odprete, in odstranite Prilogo in izberite **Izbriši**).</span><span class="sxs-lookup"><span data-stu-id="edd9a-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="edd9a-111">Če se prikaže napaka, ki pravi, da Outlook poskuša posredovati sporočilo, zaprite Outlook.</span><span class="sxs-lookup"><span data-stu-id="edd9a-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="edd9a-112">Lahko traja nekaj trenutkov za izhod.</span><span class="sxs-lookup"><span data-stu-id="edd9a-112">It may take a few moments to exit.</span></span> <span data-ttu-id="edd9a-113">Če se Outlook ne zapre, pritisnite CTRL + ALT + DELETE in izberite **Zaženi upravitelja opravil**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="edd9a-114">V upravitelju opravil izberite zavihek **procesi** , se pomaknite navzdol do možnosti Outlook. exe in izberite **Končaj proces**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="edd9a-115">Ko se Outlook zapre, ga znova zaženite in ponovite korake 2 in 3.</span><span class="sxs-lookup"><span data-stu-id="edd9a-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="edd9a-116">Ko odstranite Prilogo, kliknite **Pošlji/Prejmi** > **delo brez povezave** , da nadaljujete delo v spletu.</span><span class="sxs-lookup"><span data-stu-id="edd9a-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="edd9a-117">Sporočila se tudi zataknejo v mapi» **Odpošlji**«, ko kliknete Pošlji, vendar niste povezani.</span><span class="sxs-lookup"><span data-stu-id="edd9a-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="edd9a-118">Kliknite **Pošlji/Prejmi** in si oglejte **delovni gumb brez povezave** .</span><span class="sxs-lookup"><span data-stu-id="edd9a-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="edd9a-119">Če je modra, si izključen.</span><span class="sxs-lookup"><span data-stu-id="edd9a-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="edd9a-120">Kliknite na povezavo (gumb se obarva belo) in kliknite **Pošlji vse**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="edd9a-121">**Omogoči pošiljanje takoj, ko je priključen**</span><span class="sxs-lookup"><span data-stu-id="edd9a-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="edd9a-122">Na kartici Datoteka kliknite **možnosti**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="edd9a-123">V pogovornem oknu možnosti programa Outlook kliknite **Napredno**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="edd9a-124">V odseku Pošlji in prejmi kliknite, če želite omogočiti **pošiljanje takoj, ko je priključen**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="edd9a-125">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="edd9a-125">Click **OK**.</span></span>
 
<span data-ttu-id="edd9a-126">Za vse podrobnosti glejte:</span><span class="sxs-lookup"><span data-stu-id="edd9a-126">For full details, see:</span></span>
- [<span data-ttu-id="edd9a-127">Videoposnetek: pošiljanje ali brisanje zagozdila e-poštnega sporočila</span><span class="sxs-lookup"><span data-stu-id="edd9a-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="edd9a-128">E-pošta ostane v mapi» Odpošlji «, dokler ročno ne sprožite operacije pošiljanja/prejemanja v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="edd9a-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
