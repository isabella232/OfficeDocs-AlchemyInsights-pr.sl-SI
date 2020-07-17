---
title: Odpravljanje težav s storitvijo OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749169"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="03bf9-102">Odpravljanje težav s storitvijo OneDrive</span><span class="sxs-lookup"><span data-stu-id="03bf9-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="03bf9-103">Če se storitev OneDrive večkrat zruši, poskusite te korake za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="03bf9-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="03bf9-104">**Zagotovite, da registrski ključi niso določeni:**</span><span class="sxs-lookup"><span data-stu-id="03bf9-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="03bf9-105">Z urejevalnikom registra krmarite do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="03bf9-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="03bf9-106">Če DisableFileSyncNGSC je sedanji ter število enakih oseb v 1, plan zakleniti ter sprememba vrednost v 0.</span><span class="sxs-lookup"><span data-stu-id="03bf9-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="03bf9-107">Ročno zaženite OneDrive, tako da se bo začela</span><span class="sxs-lookup"><span data-stu-id="03bf9-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="03bf9-109">, v iskalno polje vnesite OneDrive in kliknite na namizno aplikacijo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="03bf9-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="03bf9-110">**Ponastavi OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="03bf9-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="03bf9-111">Opombe:</span><span class="sxs-lookup"><span data-stu-id="03bf9-111">Notes:</span></span>

- <span data-ttu-id="03bf9-112">Ponastavitev storitve OneDrive prekine povezavo vseh obstoječih sinhronizacijskih povezav (vključno z vašo osebno storitvijo OneDrive, če je nastavljena).</span><span class="sxs-lookup"><span data-stu-id="03bf9-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="03bf9-113">Datotek ali podatkov ne boste izgubili tako, da ponastavite OneDrive v računalniku.</span><span class="sxs-lookup"><span data-stu-id="03bf9-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="03bf9-114">**Če želite ponastaviti OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="03bf9-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="03bf9-115">Odprite pogovorno okno Zaženi tako, da pritisnete tipko Windows in R.</span><span class="sxs-lookup"><span data-stu-id="03bf9-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="03bf9-116">Vnesite% localappdata% \Microsoft\OneDrive\onedrive.exe/Ponastavi in pritisnite OK.</span><span class="sxs-lookup"><span data-stu-id="03bf9-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="03bf9-117">Na kratko se lahko prikaže okno ukaznega okna.</span><span class="sxs-lookup"><span data-stu-id="03bf9-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="03bf9-118">Ročno zaženite OneDrive, tako da se bo začela</span><span class="sxs-lookup"><span data-stu-id="03bf9-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="03bf9-120">, v iskalno polje vnesite OneDrive in kliknite na namizno aplikacijo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="03bf9-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="03bf9-121">Opombe:</span><span class="sxs-lookup"><span data-stu-id="03bf9-121">Notes:</span></span>

- <span data-ttu-id="03bf9-122">Če ste se odločili za sinhronizacijo le nekaj map pred ponastavitvijo, boste morali to storiti znova, ko je končana sinhronizacija.</span><span class="sxs-lookup"><span data-stu-id="03bf9-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="03bf9-123">Če želite več informacij, preberite [Izberite, katere mape v storitvi OneDrive želite sinhronizirati z računalnikom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="03bf9-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="03bf9-124">To boste morali dokončati za osebne storitve OneDrive in OneDrive za podjetja.</span><span class="sxs-lookup"><span data-stu-id="03bf9-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>