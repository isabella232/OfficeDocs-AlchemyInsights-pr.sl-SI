---
title: Imenik Active Directory se ne sinhronizira
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822867"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="6cc1e-102">Imenik Active Directory se ne sinhronizira</span><span class="sxs-lookup"><span data-stu-id="6cc1e-102">Active Directory not syncing</span></span>

<span data-ttu-id="6cc1e-103">Če prejemate napake pri sinhronizaciji, na primer »ni nedavne sinhronizacije«, ali pa opazite stanje sinhronizacije imenika v skrbniškem portalu za Office pravi »Nazadnje sinhronizirano pred več kot 3 dnevi«, ima AADConnect morda nepravilne nastavitve ali nezadostna dovoljenja za izvajanje sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="6cc1e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="6cc1e-104">Če znova namestite AADConnect s hitrimi nastavitvami, boste težavo morda lahko hitreje odpravili:</span><span class="sxs-lookup"><span data-stu-id="6cc1e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="6cc1e-105">[Prenesite najnovejšo različico programa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="6cc1e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="6cc1e-106">[Upoštevajte navodila za hitro namestitev.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="6cc1e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="6cc1e-107">Če želite več informacij o računih storitve AADConnect, glejte [Azure AD Connect: računi in dovoljenja.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="6cc1e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
