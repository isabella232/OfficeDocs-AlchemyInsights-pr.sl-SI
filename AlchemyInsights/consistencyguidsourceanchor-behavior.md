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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044356"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor behavior

Azure AD Povezovalnik (različica 1.1.524.0 in nato) zdaj omogoča uporabo msDS-ConsistencyGuid kot atribut sourceAnchor. Ko uporabljate to funkcijo, azure AD Povezovalnik samodejno konfigurira pravila za sinhronizacijo tako:
  
- Uporabite msDS-ConsistencyGuid kot atribut sourceAnchor za uporabniške predmete. ObjectGUID se uporablja za druge vrste predmetov.
    
- Za kateri koli dani predmet AD User na mestu uporabe, katerega atribut msDS-ConsistencyGuid ni izpolnjen, Azure AD Povezovalnik svojo vrednost objectGUID zapiše nazaj v atribut msDS-ConsistencyGuid v imeniku Active Directory na mestu uporabe. Ko je atribut msDS-ConsistencyGuid izpolnjen, azure AD Povezovalnik nato izvozi predmet v Azure AD.
    
 **Opomba:** Ko je predmet AD na mestu uporabe uvožen v Azure AD Povezovalnik (ki se uvozi v prostor povezovalnika AD in je projiciran v Metaverse), ne morete več spremeniti njegove izvorne vrednosti Zaganjalnik. Če želite določiti vrednost izvornega ključa za dani predmet AD na mestu uporabe, konfigurirajte njegov atribut msDS-ConsistencyGuid, preden se uvozi v imenik Azure AD Povezovalnik. 
  
Če želite več informacij o sourceAnchor in ConsistencyGuid, glejte: [Azure AD Povezovalnik: koncepti načrtovanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

