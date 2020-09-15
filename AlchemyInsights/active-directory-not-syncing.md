---
title: Imenik Active Directory ni sinhroniziran
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697645"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="ad76e-102">Imenik Active Directory ni sinhroniziran</span><span class="sxs-lookup"><span data-stu-id="ad76e-102">Active Directory not syncing</span></span>

<span data-ttu-id="ad76e-103">Če prejemate napake pri sinhronizaciji, na primer» ni nedavne sinhronizacije «ali obvestilo o stanju sinhronizacije imenika v skrbniškem portalu za Office, je» nazadnje sinhronizirano več kot 3 dni nazaj «, da ima AADConnect nepravilne nastavitve ali nezadostna dovoljenja za izvajanje sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="ad76e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="ad76e-104">Če znova namestite AADConnect z izrazi z izrecnimi nastavitvami, lahko hitro odpravite težavo:</span><span class="sxs-lookup"><span data-stu-id="ad76e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="ad76e-105">[Prenesite najnovejšo različico storitve AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="ad76e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="ad76e-106">[Sledite navodilom za ekspresno namestitev](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="ad76e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="ad76e-107">Če želite več informacij o računih storitve AADConnect, glejte [povezavo AZURE ad Connect: računi in dovoljenja](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="ad76e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
