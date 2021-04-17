---
title: Odpravljanje težav z zrušitve storitve OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826215"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="4f35e-102">Odpravljanje težav z zrušitve storitve OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f35e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="4f35e-103">Če se OneDrive večkrat zruši, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="4f35e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="4f35e-104">**Zagotovite, da registrski ključi niso nastavljeni:**</span><span class="sxs-lookup"><span data-stu-id="4f35e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="4f35e-105">Z urejevalnikom registra odprite HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f35e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="4f35e-106">Če je DisableFileSyncNGSC prisoten in nastavljen na 1, odprite ključ in spremenite vrednost na 0.</span><span class="sxs-lookup"><span data-stu-id="4f35e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="4f35e-107">Ročni zagon storitve OneDrive v začetnem meniju</span><span class="sxs-lookup"><span data-stu-id="4f35e-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="4f35e-109">, v iskalno polje vnesite OneDrive in kliknite namizno aplikacijo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4f35e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="4f35e-110">**Ponastavite OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="4f35e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="4f35e-111">Opombe:</span><span class="sxs-lookup"><span data-stu-id="4f35e-111">Notes:</span></span>

- <span data-ttu-id="4f35e-112">S ponastavitvijo storitve OneDrive boste prekinili vse obstoječe povezave za sinhronizacijo (tudi osebni OneDrive, če je nastavljen).</span><span class="sxs-lookup"><span data-stu-id="4f35e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="4f35e-113">S ponastavitvijo storitve OneDrive v računalniku ne boste izgubili datotek ali podatkov.</span><span class="sxs-lookup"><span data-stu-id="4f35e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="4f35e-114">**Če želite ponastaviti OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="4f35e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="4f35e-115">Odprite pogovorno okno »Zaženi« tako, da pritisnete tipko Windows in R.</span><span class="sxs-lookup"><span data-stu-id="4f35e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="4f35e-116">Vnesite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset in pritisnite V redu.</span><span class="sxs-lookup"><span data-stu-id="4f35e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="4f35e-117">Za kratek čas se lahko prikaže ukazno okno.</span><span class="sxs-lookup"><span data-stu-id="4f35e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="4f35e-118">Ročni zagon storitve OneDrive v začetnem meniju</span><span class="sxs-lookup"><span data-stu-id="4f35e-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="4f35e-120">, v iskalno polje vnesite OneDrive in kliknite namizno aplikacijo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4f35e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="4f35e-121">Opombe:</span><span class="sxs-lookup"><span data-stu-id="4f35e-121">Notes:</span></span>

- <span data-ttu-id="4f35e-122">Če ste se odločili, da pred ponastavitvijo sinhronizirate le nekatere mape, boste morali to storiti znova, ko bo sinhronizacija končana.</span><span class="sxs-lookup"><span data-stu-id="4f35e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="4f35e-123">Če [želite več informacij, preberite Izberite mape storitve OneDrive, ki jih želite sinhronizirati](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   z računalnikom.</span><span class="sxs-lookup"><span data-stu-id="4f35e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="4f35e-124">To boste morali dokončati za osebni OneDrive in OneDrive za podjetja.</span><span class="sxs-lookup"><span data-stu-id="4f35e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>