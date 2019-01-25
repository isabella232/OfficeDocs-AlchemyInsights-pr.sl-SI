---
title: ConsistencyGuid / sourceAnchor vedenje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498534"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor vedenje

Sinje AD Connect (različica 1.1.524.0 in je po) zdaj omogoča uporabo kostno-ConsistencyGuid kot atribut sourceAnchor. Pri uporabi te funkcije, Azure AD povezavo samodejno konfigurira pravili sinhronizacije za:
  
- Uporabite kostno-ConsistencyGuid kot atribut sourceAnchor za uporabniški predmeti. »ObjectGUID «se uporablja za druge vrste predmetov.
    
- Za vse krajevne AD uporabniški predmet katerih kostno-ConsistencyGuid atribut ni vneseno, Azure AD povezavo piše vrednost »objectGUID« nazaj do kostno-ConsistencyGuid atributa v krajevnem imeniku Active Directory. Po kostno-ConsistencyGuid atribut je poseljena, Azure AD povezavo nato izvoz predmeta v sinje AD.
    
 **Opomba:** Enkrat krajevni predmet AD je uvozi Azure AD povezavo (namreč uvažajo v prostor za konektor AD in projicirani v Metaverse), svoje sourceAnchor vrednosti ne morete več spremeniti. Določite vrednost sourceAnchor je glede krajevne AD predmet, nastavite njen atribut kostno-ConsistencyGuid, preden jo uvozite v Azure AD povezavo. 
  
Če želite več informacij o SourceAnchor in ConsistencyGuid, bodite pozorni na naslednje: [Azure AD povezavo: oblikovalski](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

