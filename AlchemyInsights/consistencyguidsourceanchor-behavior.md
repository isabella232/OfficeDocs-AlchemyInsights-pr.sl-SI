---
title: ConsistencyGuid / sourceAnchor vedenje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753118"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="2a6d8-102">ConsistencyGuid / sourceAnchor vedenje</span><span class="sxs-lookup"><span data-stu-id="2a6d8-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="2a6d8-103">Sinje AD Connect (različica 1.1.524.0 in je po) zdaj omogoča uporabo kostno-ConsistencyGuid kot atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="2a6d8-104">Pri uporabi te funkcije, Azure AD povezavo samodejno konfigurira pravili sinhronizacije za:</span><span class="sxs-lookup"><span data-stu-id="2a6d8-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="2a6d8-105">Uporabite kostno-ConsistencyGuid kot atribut sourceAnchor za uporabniški predmeti.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="2a6d8-106">»ObjectGUID «se uporablja za druge vrste predmetov.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="2a6d8-107">Za vse krajevne AD uporabniški predmet katerih kostno-ConsistencyGuid atribut ni vneseno, Azure AD povezavo piše vrednost »objectGUID« nazaj do kostno-ConsistencyGuid atributa v krajevnem imeniku Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="2a6d8-108">Po kostno-ConsistencyGuid atribut je poseljena, Azure AD povezavo nato izvoz predmeta v sinje AD.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="2a6d8-109">**Opomba:** Enkrat krajevni predmet AD je uvozi Azure AD povezavo (namreč uvažajo v prostor za konektor AD in projicirani v Metaverse), svoje sourceAnchor vrednosti ne morete več spremeniti.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="2a6d8-110">Določite vrednost sourceAnchor je glede krajevne AD predmet, nastavite njen atribut kostno-ConsistencyGuid, preden jo uvozite v Azure AD povezavo.</span><span class="sxs-lookup"><span data-stu-id="2a6d8-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="2a6d8-111">Če želite več informacij o SourceAnchor in ConsistencyGuid, bodite pozorni na naslednje: [Azure AD povezavo: oblikovalski](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="2a6d8-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

