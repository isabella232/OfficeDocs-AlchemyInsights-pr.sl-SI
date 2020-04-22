---
title: Konsistenciin GUID/sourceAnchor obnašanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705749"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Konsistenciin GUID/sourceAnchor obnašanje

Azure AD Connect (različica 1.1.524.0 in pozneje) zdaj olajšuje uporabo msDS-doslednosti GUID kot atribut sourceAnchor. Ko uporabljate to funkcijo, Azure AD Connect samodejno konfigurira pravila sinhronizacije tako, da:
  
- Uporabite msDS-Konsistenciuuguid kot atribut sourceAnchor za uporabniške predmete. ObjectGUID se uporablja za druge vrste predmetov.
    
- V katerem koli danem krajevnem uporabniškem predmetu AD, katerega atribut msDS-Konsistencyguid ni poseljen, Azure AD Connect zapiše svojo vrednost objectGUID nazaj v atribut msDS-Konsistencyguid v krajevnem imeniku Active Directory. Ko je atribut msDS-Konsistencyguid naseljen, Azure AD Connect nato izvozi predmet v Azure AD.
    
 **Opomba:** Ko se krajevni predmet oglasa uvozi v Azure AD Connect (to je uvoženo v prostor AD Connector in napovedano v metaverse), ne morete več spreminjati vrednosti sourceAnchor. Če želite določiti vrednost sourceAnchor za dani krajevni predmet oglasa, konfigurirajte atribut msDS-Konsistencyguid, preden ga uvozite v Azure AD Connect. 
  
Če želite več informacij o SourceAnchor in doslednosti GUID-a, glejte naslednje: [AZURE ad Connect: oblikovalni koncepti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

