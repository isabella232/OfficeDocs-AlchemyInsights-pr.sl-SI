---
title: Navidezna konfiguracija s storitvami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885650"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="3c7d6-102">Navidezna konfiguracija s storitvami</span><span class="sxs-lookup"><span data-stu-id="3c7d6-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="3c7d6-103">Navidezna konfiguracija s storitvijo storitev za ZVOČNO premišljene domene vključuje te korake:</span><span class="sxs-lookup"><span data-stu-id="3c7d6-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="3c7d6-104">Preverjanje zdravja domene na portalu Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="3c7d6-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="3c7d6-105">Preverjanje NSG za pravila, ki blokirajo vrata, potrebna za sinhronizacijo v domenskih storitvah storitve Azure AD v portalu https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="3c7d6-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="3c7d6-106">Zagotovite, da je navidezno omrežje razporejeno v isti regiji Azure kot domena storitve Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="3c7d6-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="3c7d6-107">Zagotavljanje, da nimate obstoječe domene z istim imenom domene, ki je na voljo v navideznem omrežju.</span><span class="sxs-lookup"><span data-stu-id="3c7d6-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="3c7d6-108">Če želite več informacij o načrtovanju načrtovanja v navideznem omrežju Azure, da boste podpirali storitve storitev s pozdravnimi domenami, glejte [navidezna omrežna](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)</span><span class="sxs-lookup"><span data-stu-id="3c7d6-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

