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
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36527059"
---
# <a name="error-attributevaluemustbeunique"></a>Napaka: AttributeValueMustBeUnique

Najpogostejši razlog za atribut» AttributeValueMustBeUnique «je dva predmeta z različnimi SourceAnchor (immutableId) imajo enako vrednost za atribute ProxyAddresses in/ali UserPrincipalName. Če želite popraviti napako» AttributeValueMustBeUnique «:
  
1. Prepoznajte podvojeni proxyAddresses, userPrincipalName ali drugo vrednost atributa, ki povzroča napako. Ugotovite tudi, kateri dve (ali več) predmeti so vpleteni v konflikt. Poročilo, ki ga ustvari Azure AD Connect Health za sinhronizacijo, vam lahko pomaga prepoznati dva predmeta.
    
2. Ugotovite, kateri predmet mora še naprej imeti Podvojena vrednost in kateri predmet ne bi smel.
    
3. Odstranite Podvojena vrednost iz predmeta, ki ne bi smel imeti te vrednosti. Upoštevajte, da bi morali spremeniti v imeniku, od koder je predmet izvirajo. V nekaterih primerih boste morda morali izbrisati enega od predmetov v sporu.
    
4. Če ste naredili spremembo v prostorih oglasa, naj Azure AD Connect sinhronizira spremembo napake, da se določi.
    

