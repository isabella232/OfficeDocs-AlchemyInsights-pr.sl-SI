---
title: Zaženite Windows Memory diagnostika v operacijskem sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358294"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="3edd8-102">Zaženite Windows Memory diagnostika v operacijskem sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="3edd8-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="3edd8-103">Če se Windows in aplikacije v računalniku zrušijo, zamrzujejo ali delujejo na nestabilen način, imate morda težave s pomnilnikom računalnika (RAM-a).</span><span class="sxs-lookup"><span data-stu-id="3edd8-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="3edd8-104">Če želite preveriti težave z RAM-om računalnika, lahko zaženete diagnostiko pomnilnika sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="3edd8-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="3edd8-105">V iskalno polje v opravilni vrstici vnesite **diagnostično pomnilniško kartico**in nato izberite **diagnostično pomnilniško kartico Windows**.</span><span class="sxs-lookup"><span data-stu-id="3edd8-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="3edd8-106">Če želite zagnati diagnostiko, se mora računalnik znova zagnati.</span><span class="sxs-lookup"><span data-stu-id="3edd8-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="3edd8-107">Vi življati predkupna pravica v zopet začeti takoj (prosim zaščititi vaš opus ter blizu plan listina ter črka e-verižna srajca prvi), ali tabela spoznati bolezen teči automatically naslednji čas PC zopet začeti:</span><span class="sxs-lookup"><span data-stu-id="3edd8-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostika pomnilnika sistema Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="3edd8-109">Ko se računalnik znova zažene, se bo **orodje za diagnostiko pomnilnika sistema Windows** samodejno zagnali.</span><span class="sxs-lookup"><span data-stu-id="3edd8-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="3edd8-110">Stanje in napredek bosta prikazana kot diagnostična vaja, vi pa imate možnost preklica diagnostike tako, da na tipkovnici udarjajte tipko **ESC** .</span><span class="sxs-lookup"><span data-stu-id="3edd8-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="3edd8-111">Ko je diagnostika končana, se Windows zažene normalno.</span><span class="sxs-lookup"><span data-stu-id="3edd8-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="3edd8-112">Takoj po vnovičnem zagonu, ko se prikaže namizje, se prikaže obvestilo (poleg ikone **središča za opravila** v opravilni vrstici), da označite, ali so bile najdene napake v pomnilniku.</span><span class="sxs-lookup"><span data-stu-id="3edd8-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="3edd8-113">Na primer:</span><span class="sxs-lookup"><span data-stu-id="3edd8-113">For example:</span></span>

<span data-ttu-id="3edd8-114">Tukaj je ikona središča za opravila:</span><span class="sxs-lookup"><span data-stu-id="3edd8-114">Here's the Action Center icon:</span></span> ![Ikona središča za opravila](media/action-center-icon.png) 

<span data-ttu-id="3edd8-116">In vzorčno obvestilo:</span><span class="sxs-lookup"><span data-stu-id="3edd8-116">And a sample notification:</span></span> ![Brez pomnilniških napak](media/no-memory-errors.png)

<span data-ttu-id="3edd8-118">Če ste obvestilo zamudili, lahko v opravilni vrstici izberete ikono **središče za opravila** , da prikažete središče za **opravila** in si ogledate seznam obvestil, ki jih je mogoče zapisati.</span><span class="sxs-lookup"><span data-stu-id="3edd8-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="3edd8-119">Če želite pregledati podrobne informacije, v iskalno polje v opravilni vrstici vnesite **dogodek** in nato izberite **Pregledovalnik dogodkov**.</span><span class="sxs-lookup"><span data-stu-id="3edd8-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="3edd8-120">V levem podoknu **pregledovalnika dogodkov**krmarite do **dnevnikov sistema Windows > System**.</span><span class="sxs-lookup"><span data-stu-id="3edd8-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="3edd8-121">V desnem podoknu skenirajte seznam med iskanjem v **izvornem** stolpcu, dokler ne vidite dogodkov z izvorno vrednostjo **memorydiagnostics-rezultati**.</span><span class="sxs-lookup"><span data-stu-id="3edd8-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="3edd8-122">Označite vsak tak dogodek in si oglejte informacije o rezultatih v polju pod zavihkom **splošno** pod seznamom.</span><span class="sxs-lookup"><span data-stu-id="3edd8-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
