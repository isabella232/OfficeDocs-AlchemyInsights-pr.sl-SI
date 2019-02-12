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
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927693"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor vedenje

Sinje AD Connect (različica 1.1.524.0 in je po) zdaj omogoča uporabo kostno-ConsistencyGuid kot atribut sourceAnchor. Pri uporabi te funkcije, Azure AD povezavo samodejno konfigurira pravili sinhronizacije za:
  
- Uporabite kostno-ConsistencyGuid kot atribut sourceAnchor za uporabniški predmeti. »ObjectGUID «se uporablja za druge vrste predmetov.
    
- Za vse krajevne AD uporabniški predmet katerih kostno-ConsistencyGuid atribut ni vneseno, Azure AD povezavo piše vrednost »objectGUID« nazaj do kostno-ConsistencyGuid atributa v krajevnem imeniku Active Directory. Po kostno-ConsistencyGuid atribut je poseljena, Azure AD povezavo nato izvoz predmeta v sinje AD.
    
 **Opomba:** Enkrat krajevni predmet AD je uvozi Azure AD povezavo (namreč uvažajo v prostor za konektor AD in projicirani v Metaverse), svoje sourceAnchor vrednosti ne morete več spremeniti. Določite vrednost sourceAnchor je glede krajevne AD predmet, nastavite njen atribut kostno-ConsistencyGuid, preden jo uvozite v Azure AD povezavo. 
  
Če želite več informacij o SourceAnchor in ConsistencyGuid, bodite pozorni na naslednje: [Azure AD povezavo: oblikovalski](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

