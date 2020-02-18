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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091766"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="3f077-102">Pravilnika» Allowselfservicenabava «ni mogoče nastaviti ali si ogledati</span><span class="sxs-lookup"><span data-stu-id="3f077-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="3f077-103">Ko poskušate nastaviti ali si ogledati pravilnik Allowselfservicenabava, se prikaže to sporočilo o napaki:</span><span class="sxs-lookup"><span data-stu-id="3f077-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="3f077-104">*HandleError: ne zadostovati v rešitev zmnožek zvitost s PolicyId ' Allowselfservicenabava ', ErrorMessage-osnovna povezava je bila zaprta: Prišlo je do nepričakovane napake pri pošiljanju.*</span><span class="sxs-lookup"><span data-stu-id="3f077-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="3f077-105">To je lahko posledica starejše različice varnosti transportnega sloja (TLS).</span><span class="sxs-lookup"><span data-stu-id="3f077-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="3f077-106">Če želite povezati storitev MSCommerce, morate uporabiti TLS 1,2 ali več.</span><span class="sxs-lookup"><span data-stu-id="3f077-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="3f077-107">Če želite omogočiti/nastaviti protokol TLS na 1,2, preverite in poskusite znova, poskusite naslednje korake.</span><span class="sxs-lookup"><span data-stu-id="3f077-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="3f077-108">V ukazni poziv PowerShell (PS C:\) vnesite naslednji ukaz, da NASTAVITE protokol TLS na različico 1,2:</span><span class="sxs-lookup"><span data-stu-id="3f077-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="3f077-109">\[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="3f077-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="3f077-110">Preverite protokole TLS, ki jih uporabljate, z naslednjim ukazom:</span><span class="sxs-lookup"><span data-stu-id="3f077-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="3f077-111">\[Net. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="3f077-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="3f077-112">Po potrebi znova poskusite ukaze Get ali Update.</span><span class="sxs-lookup"><span data-stu-id="3f077-112">Retry the Get or Update commands as needed.</span></span>

