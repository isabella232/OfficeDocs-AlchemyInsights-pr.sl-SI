---
title: Pravilnika AllowSelfServicePurchase ni mogoče nastaviti ali si ogledati
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735215"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="1bf0c-102">Pravilnika AllowSelfServicePurchase ni mogoče nastaviti ali si ogledati</span><span class="sxs-lookup"><span data-stu-id="1bf0c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="1bf0c-103">Pri poskusu nastavljanja ali ogleda pravilnika AllowSelfServicePurchase se prikaže to sporočilo o napaki:</span><span class="sxs-lookup"><span data-stu-id="1bf0c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="1bf0c-104">*HandleError: ni bilo mogoče pridobiti pravilnika o izdelku z PolicyId» AllowSelfServicePurchase «,» errorMessage «– osnovna povezava je bila zaprta: Nepričakovana napaka pri pošiljanju.*</span><span class="sxs-lookup"><span data-stu-id="1bf0c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="1bf0c-105">To je morda zaradi starejše različice varnosti transportne plasti (TLS).</span><span class="sxs-lookup"><span data-stu-id="1bf0c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="1bf0c-106">Če želite vzpostaviti povezavo s storitvijo MSCommerce, morate uporabiti TLS 1,2 ali novejšo.</span><span class="sxs-lookup"><span data-stu-id="1bf0c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="1bf0c-107">Upoštevajte spodnja navodila za omogočanje/nastavitev protokola TLS v 1,2, preverjanje in vnovičen poskus.</span><span class="sxs-lookup"><span data-stu-id="1bf0c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="1bf0c-108">V ukazni vrstici lupine PowerShell (PS C: \) vnesite ta ukaz, da nastavite protokol TLS na različico 1,2:</span><span class="sxs-lookup"><span data-stu-id="1bf0c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="1bf0c-109">Preverjanje protokola TLS v uporabi s tem ukazom:</span><span class="sxs-lookup"><span data-stu-id="1bf0c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="1bf0c-110">Po potrebi znova poskusite izvesti ukaze Get ali Update.</span><span class="sxs-lookup"><span data-stu-id="1bf0c-110">Retry the Get or Update commands as needed.</span></span>

