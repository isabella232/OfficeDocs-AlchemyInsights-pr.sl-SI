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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor behavior

Azure AD Connect (različica 1.1.524.0 in po tem) zdaj omogoča uporabo msDS-ConsistencyGuid kot atribut sourceAnchor. Ko uporabljate to funkcijo, Azure AD Connect samodejno konfigurira pravila za sinhronizacijo tako:
  
- Uporabite msDS-ConsistencyGuid kot atribut sourceAnchor za uporabniške predmete. ObjectGUID se uporablja za druge vrste predmetov.
    
- Za kateri koli dani predmet AD User na mestu uporabe, katerega atribut msDS-ConsistencyGuid ni izpolnjen, Azure AD Connect zapiše vrednost objectGUID nazaj v atribut msDS-ConsistencyGuid v imeniku Active Directory na mestu uporabe. Ko je atribut msDS-ConsistencyGuid izpolnjen, Azure AD Connect izvozi predmet v Azure AD.
    
 **Opomba:** Ko je predmet AD na mestu uporabe uvožen v Azure AD Connect (ki je uvožen v prostor povezovalnika AD in projiciran v Metaverse), ne morete več spremeniti njegove izvorne vrednosti za zaganjalnik. Če želite določiti vrednost izvornega ključa za dani predmet AD na mestu uporabe, konfigurirajte njegov atribut msDS-ConsistencyGuid, preden ga uvozite v Azure AD Connect. 
  
Če želite več informacij o sourceAnchor in ConsistencyGuid, glejte: [Azure AD Connect: koncepti načrtovanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

