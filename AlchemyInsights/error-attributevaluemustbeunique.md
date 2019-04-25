---
title: Napaka AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402719"
---
# <a name="error-attributevaluemustbeunique"></a>Napaka: AttributeValueMustBeUnique

Najpogostejši razlog za AttributeValueMustBeUnique napaka je dveh predmetov z različnimi SourceAnchor (immutableId) imajo enako vrednost za ProxyAddresses in/ali UserPrincipalName atribute. Popraviti napako AttributeValueMustBeUnique:
  
1. Prepoznavanje podvojiti proxyAddresses, userPrincipalName ali druge vrednosti atributa, ki povzroča napako. Tudi opredelijo dva (ali več) predmetov, ki so vključeni v spor. Poročila, ki ga Azure AD povezavo zdravje za sinhronizacijo lahko prepoznate dveh predmetov.
    
2. Opredelitev predmeta, ki naj imajo še naprej podvojene vrednosti in predmeta, ki ne bi smela.
    
3. Odstranite podvojene vrednosti iz predmeta, ki ne bi smel imeti to vrednost. Upoštevajte, da morate narediti spremembo v imenik, kjer je predmet izvirajo iz. V nekaterih primerih boste morali izbrisati enega od predmetov v konflikt.
    
4. Če ste naredili spremembe v prostorih na oglas, naj Azure AD povezave sinhronizirati sprememb za napake, ki se določi.
    

