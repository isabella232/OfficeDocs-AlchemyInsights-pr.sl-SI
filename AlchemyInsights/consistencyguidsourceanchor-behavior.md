---
title: Delovanje ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756299"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="a4de5-102">Delovanje ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="a4de5-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="a4de5-103">Azure AD Connect (različica 1.1.524.0 in nato) zdaj olajšuje uporabo kostno-ConsistencyGuid kot sourceAnchor atributa.</span><span class="sxs-lookup"><span data-stu-id="a4de5-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="a4de5-104">Ko uporabite to funkcijo, Azure AD Connect samodejno konfigurira pravila sinhronizacije:</span><span class="sxs-lookup"><span data-stu-id="a4de5-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="a4de5-105">Uporabite varnostni list – ConsistencyGuid kot atribut sourceAnchor za uporabniške predmete.</span><span class="sxs-lookup"><span data-stu-id="a4de5-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="a4de5-106">ObjectGUID se uporablja za druge vrste predmetov.</span><span class="sxs-lookup"><span data-stu-id="a4de5-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="a4de5-107">Za kateri koli predmet uporabnika na mestu uporabe, ki ni poseljen z atributom» ConsistencyGuid «, Azure AD Connect poveže svojo objectGUID vrednost v atribut» kostno-ConsistencyGuid «v imeniku Active Directory na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="a4de5-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="a4de5-108">Ko je lastnost» kostno-ConsistencyGuid «izpolnjena, je Azure AD Connect nato izvoz predmeta v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a4de5-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="a4de5-109">**Opomba:** Ko je predmet OGLASa na mestu uporabe uvožen v strežnik Azure AD Connect (ki je uvožen v prostor za konektor OGLASa in načrtovan v metaverse), ne morete več spremeniti njegove sourceAnchor vrednosti.</span><span class="sxs-lookup"><span data-stu-id="a4de5-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="a4de5-110">Če želite določiti vrednost sourceAnchor za dani predmet na mestu uporabe, konfigurirajte njegov atribut» kostno-ConsistencyGuid «, preden ga uvozite v povezavo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a4de5-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="a4de5-111">Če želite več informacij o SourceAnchor in ConsistencyGuid, glejte naslednje: [AZURE ad Connect: koncepti načrta](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="a4de5-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

