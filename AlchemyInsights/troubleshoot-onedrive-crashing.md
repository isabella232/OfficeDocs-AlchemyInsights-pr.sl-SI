---
title: Odpravljanje težav z OneDrive zruši
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665014"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="e7c8c-102">Odpravljanje težav z OneDrive zruši</span><span class="sxs-lookup"><span data-stu-id="e7c8c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="e7c8c-103">Če se OneDrive večkrat zruši, poskusite s temi koraki za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="e7c8c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="e7c8c-104">**Zagotovite, da registrski ključi niso nastavljeni:**</span><span class="sxs-lookup"><span data-stu-id="e7c8c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="e7c8c-105">Uporaba urejevalnika registra se pomaknite do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="e7c8c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="e7c8c-106">Če je argument» DisableFileSyncNGSC «prisoten in nastavljen na 1, odprite tipko in spremenite vrednost na 0.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="e7c8c-107">Ročno zaženite OneDrive tako, da začnete</span><span class="sxs-lookup"><span data-stu-id="e7c8c-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e7c8c-109">, v iskalno polje vnesite OneDrive in nato kliknite OneDrive namizni program.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e7c8c-110">**Ponastavi OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e7c8c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="e7c8c-111">Opombe</span><span class="sxs-lookup"><span data-stu-id="e7c8c-111">Notes:</span></span>

- <span data-ttu-id="e7c8c-112">S ponastavitvijo OneDrive prekinete povezavo vseh obstoječih sinhronizacijskih povezav (vključno z vašim osebnim OneDrive, če ste nastavili).</span><span class="sxs-lookup"><span data-stu-id="e7c8c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="e7c8c-113">Datotek ali podatkov ne boste izgubili s ponastavitvijo OneDrive v računalniku.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="e7c8c-114">**Če želite ponastaviti OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e7c8c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="e7c8c-115">Odprite pogovorno okno za zagon tako, da pritisnete tipko Windows in R.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="e7c8c-116">Vnesite% localappdata% \Microsoft\OneDrive\onedrive.exe/reset in pritisnite v redu.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="e7c8c-117">Ukazno okno se lahko prikaže na kratko.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="e7c8c-118">Ročno zaženite OneDrive tako, da začnete</span><span class="sxs-lookup"><span data-stu-id="e7c8c-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e7c8c-120">, v iskalno polje vnesite OneDrive in nato kliknite OneDrive namizni program.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e7c8c-121">Opombe</span><span class="sxs-lookup"><span data-stu-id="e7c8c-121">Notes:</span></span>

- <span data-ttu-id="e7c8c-122">Če ste izbrali sinhronizacijo le nekaterih map pred ponastavitvijo, boste morali to narediti znova, ko bo sinhronizacija dokončana.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="e7c8c-123">Če želite več informacij, preberite [izbiranje, katere OneDrive mape želite sinhronizirati z računalnikom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="e7c8c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="e7c8c-124">To boste morali dokončati za osebne OneDrive in OneDrive za podjetja.</span><span class="sxs-lookup"><span data-stu-id="e7c8c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>