---
title: Pravilnika» Allowselfservicenabava «ni mogoče nastaviti ali si ogledati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158577"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="e8e88-102">Pravilnika» Allowselfservicenabava «ni mogoče nastaviti ali si ogledati</span><span class="sxs-lookup"><span data-stu-id="e8e88-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="e8e88-103">Ko poskušate nastaviti ali si ogledati pravilnik Allowselfservicenabava, se prikaže to sporočilo o napaki:</span><span class="sxs-lookup"><span data-stu-id="e8e88-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="e8e88-104">*HandleError: ne zadostovati v rešitev zmnožek zvitost s PolicyId ' Allowselfservicenabava ', ErrorMessage-osnovna povezava je bila zaprta: Prišlo je do nepričakovane napake pri pošiljanju.*</span><span class="sxs-lookup"><span data-stu-id="e8e88-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="e8e88-105">To je lahko posledica starejše različice varnosti transportnega sloja (TLS).</span><span class="sxs-lookup"><span data-stu-id="e8e88-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="e8e88-106">Če želite povezati storitev MSCommerce, morate uporabiti TLS 1,2 ali več.</span><span class="sxs-lookup"><span data-stu-id="e8e88-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="e8e88-107">Če želite omogočiti/nastaviti protokol TLS na 1,2, preverite in poskusite znova, poskusite naslednje korake.</span><span class="sxs-lookup"><span data-stu-id="e8e88-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="e8e88-108">V ukazni poziv PowerShell (PS C:\) vnesite naslednji ukaz, da NASTAVITE protokol TLS na različico 1,2:</span><span class="sxs-lookup"><span data-stu-id="e8e88-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="e8e88-109">Preverite protokole TLS, ki jih uporabljate, z naslednjim ukazom:</span><span class="sxs-lookup"><span data-stu-id="e8e88-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="e8e88-110">Po potrebi znova poskusite ukaze Get ali Update.</span><span class="sxs-lookup"><span data-stu-id="e8e88-110">Retry the Get or Update commands as needed.</span></span>

