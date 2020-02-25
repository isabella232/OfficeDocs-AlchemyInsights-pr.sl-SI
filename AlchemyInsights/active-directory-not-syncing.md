---
title: Active Directory ni sinhroniziranje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265272"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="469a4-102">Active Directory ni sinhroniziranje</span><span class="sxs-lookup"><span data-stu-id="469a4-102">Active Directory not syncing</span></span>

<span data-ttu-id="469a4-103">Če prejemate napake pri sinhronizaciji, na primer» ni nedavne sinhronizacije «ali opazite stanje sinhronizacije imenika v skrbniškem portalu za Office, piše» nazadnje sinhroniziran pred več kot tremi dnevi «, je morda to, da ima AADConnect nepravilne nastavitve ali ni dovolj dovoljenja za izvajanje sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="469a4-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="469a4-104">Ponovna namestitev AADConnect z uporabo hitrih nastavitev lahko hitro reši težavo:</span><span class="sxs-lookup"><span data-stu-id="469a4-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="469a4-105">[Prenesite najnovejšo različico AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="469a4-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="469a4-106">[Sledite navodilom za ekspresno namestitev](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="469a4-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="469a4-107">Če želite več informacij o računih storitev AADConnect, glejte [AZURE ad Connect: računi in dovoljenja](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="469a4-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
