---
title: ConsistencyGuid/sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817008"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="a24cc-102">ConsistencyGuid/sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="a24cc-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="a24cc-103">Azure AD Connect (različica 1.1.524.0 in po tem) zdaj omogoča uporabo msDS-ConsistencyGuid kot atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="a24cc-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="a24cc-104">Ko uporabljate to funkcijo, Azure AD Connect samodejno konfigurira pravila za sinhronizacijo tako:</span><span class="sxs-lookup"><span data-stu-id="a24cc-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="a24cc-105">Uporabite msDS-ConsistencyGuid kot atribut sourceAnchor za uporabniške predmete.</span><span class="sxs-lookup"><span data-stu-id="a24cc-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="a24cc-106">ObjectGUID se uporablja za druge vrste predmetov.</span><span class="sxs-lookup"><span data-stu-id="a24cc-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="a24cc-107">Za kateri koli dani predmet AD User na mestu uporabe, katerega atribut msDS-ConsistencyGuid ni izpolnjen, Azure AD Connect zapiše vrednost objectGUID nazaj v atribut msDS-ConsistencyGuid v imeniku Active Directory na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="a24cc-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="a24cc-108">Ko je atribut msDS-ConsistencyGuid izpolnjen, Azure AD Connect izvozi predmet v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a24cc-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="a24cc-109">**Opomba:** Ko je predmet AD na mestu uporabe uvožen v Azure AD Connect (ki je uvožen v prostor povezovalnika AD in projiciran v Metaverse), ne morete več spremeniti njegove izvorne vrednosti za zaganjalnik.</span><span class="sxs-lookup"><span data-stu-id="a24cc-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="a24cc-110">Če želite določiti vrednost izvornega ključa za dani predmet AD na mestu uporabe, konfigurirajte njegov atribut msDS-ConsistencyGuid, preden ga uvozite v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a24cc-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="a24cc-111">Če želite več informacij o sourceAnchor in ConsistencyGuid, glejte: [Azure AD Connect: koncepti načrtovanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="a24cc-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

