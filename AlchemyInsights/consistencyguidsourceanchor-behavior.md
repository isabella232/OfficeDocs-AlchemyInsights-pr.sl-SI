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
# <a name="consistencyguid--sourceanchor-behavior"></a>Delovanje ConsistencyGuid/sourceAnchor

Azure AD Connect (različica 1.1.524.0 in nato) zdaj olajšuje uporabo kostno-ConsistencyGuid kot sourceAnchor atributa. Ko uporabite to funkcijo, Azure AD Connect samodejno konfigurira pravila sinhronizacije:
  
- Uporabite varnostni list – ConsistencyGuid kot atribut sourceAnchor za uporabniške predmete. ObjectGUID se uporablja za druge vrste predmetov.
    
- Za kateri koli predmet uporabnika na mestu uporabe, ki ni poseljen z atributom» ConsistencyGuid «, Azure AD Connect poveže svojo objectGUID vrednost v atribut» kostno-ConsistencyGuid «v imeniku Active Directory na mestu uporabe. Ko je lastnost» kostno-ConsistencyGuid «izpolnjena, je Azure AD Connect nato izvoz predmeta v Azure AD.
    
 **Opomba:** Ko je predmet OGLASa na mestu uporabe uvožen v strežnik Azure AD Connect (ki je uvožen v prostor za konektor OGLASa in načrtovan v metaverse), ne morete več spremeniti njegove sourceAnchor vrednosti. Če želite določiti vrednost sourceAnchor za dani predmet na mestu uporabe, konfigurirajte njegov atribut» kostno-ConsistencyGuid «, preden ga uvozite v povezavo Azure AD Connect. 
  
Če želite več informacij o SourceAnchor in ConsistencyGuid, glejte naslednje: [AZURE ad Connect: koncepti načrta](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

