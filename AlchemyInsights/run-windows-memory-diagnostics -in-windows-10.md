---
title: Zagon diagnostike pomnilnika sistema Windows v sistemu Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826683"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="ce640-102">Zagon diagnostike pomnilnika sistema Windows v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="ce640-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="ce640-103">Če se Windows in aplikacije v računalniku zrušijo, zamrznejo ali delujejo nestabilen, imate morda težave s pomnilnikom računalnika (RAM).</span><span class="sxs-lookup"><span data-stu-id="ce640-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="ce640-104">Zaženete lahko diagnostiko pomnilnika v sistemu Windows in preverite težave z RAM-om računalnika.</span><span class="sxs-lookup"><span data-stu-id="ce640-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="ce640-105">V iskalno polje v opravilni vrstici vnesite **diagnostika pomnilnika** in nato izberite **Diagnostika pomnilnika sistema Windows**.</span><span class="sxs-lookup"><span data-stu-id="ce640-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="ce640-106">Če želite zagnati diagnostiko, morate računalnik znova zagnati.</span><span class="sxs-lookup"><span data-stu-id="ce640-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="ce640-107">Na voljo je možnost za takojšni vnovični zagon (shranite svoje delo in najprej zaprite dokumente in e-poštna sporočila) ali pa načrtujte samodejno izvajanje diagnostike ob naslednjem ponovnem zagonu računalnika:</span><span class="sxs-lookup"><span data-stu-id="ce640-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostika pomnilnika sistema Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="ce640-109">Ko se računalnik znova zažene, se orodje **za diagnostiko pomnilnika** sistema Windows zažene samodejno.</span><span class="sxs-lookup"><span data-stu-id="ce640-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="ce640-110">Stanje in napredek bosta prikazana med izvajanjem diagnostike, diagnostiko pa lahko prekličete tako, da pritisnete tipko **ESC** na tipkovnici.</span><span class="sxs-lookup"><span data-stu-id="ce640-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="ce640-111">Ko je diagnostika končana, se sistem Windows zažene normalno.</span><span class="sxs-lookup"><span data-stu-id="ce640-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="ce640-112">Takoj po ponovnem zagonu, ko se prikaže namizje, se prikaže obvestilo (ob ikoni središča za opravila v opravilni vrstici), ki označuje, ali je prišlo do napak v pomnilniku. </span><span class="sxs-lookup"><span data-stu-id="ce640-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="ce640-113">Na primer:</span><span class="sxs-lookup"><span data-stu-id="ce640-113">For example:</span></span>

<span data-ttu-id="ce640-114">Tukaj je ikona središča za opravila:</span><span class="sxs-lookup"><span data-stu-id="ce640-114">Here's the Action Center icon:</span></span> ![Ikona središča za opravila](media/action-center-icon.png) 

<span data-ttu-id="ce640-116">In vzorčno obvestilo:</span><span class="sxs-lookup"><span data-stu-id="ce640-116">And a sample notification:</span></span> ![Ni napak v pomnilniku](media/no-memory-errors.png)

<span data-ttu-id="ce640-118">Če ste izbrali obvestilo,  lahko izberete ikono središče  za opravila v opravilni vrstici, da prikažete središče za opravila in si ogledate seznam obvestil, po ki se jih lahko premikate.</span><span class="sxs-lookup"><span data-stu-id="ce640-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="ce640-119">Če si želite ogledati podrobne informacije, **vnesite** dogodek v iskalno polje v opravilni vrstici, nato pa izberite **Pregledovalnik dogodkov.**</span><span class="sxs-lookup"><span data-stu-id="ce640-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="ce640-120">V levem **podoknu pregledovalnika** dogodkov se pomaknite v okno Dnevniki **> Windows.**</span><span class="sxs-lookup"><span data-stu-id="ce640-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="ce640-121">V desnem podoknu preglejte seznam, medtem  ko si ogledujete stolpec Vir, dokler ne vidite dogodkov z vrednostjo Source value **MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="ce640-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="ce640-122">Označite vsak tak dogodek in si oglejte informacije o rezultatu v polju pod **zavihkom** Splošno pod seznamom.</span><span class="sxs-lookup"><span data-stu-id="ce640-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
