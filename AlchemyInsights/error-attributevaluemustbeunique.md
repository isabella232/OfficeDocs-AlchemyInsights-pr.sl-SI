---
title: Napaka AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709167"
---
# <a name="error-attributevaluemustbeunique"></a>Napaka: AttributeValueMustBeUnique

Najpogostejši vzrok za napako AttributeValueMustBeUnique je dva predmeta z različnima SourceAnchor (immutableId) imata enako vrednost za ProxyAddresses in/ali UserPrincipalName atribute. Če želite odpraviti napako AttributeValueMustBeUnique:
  
1. Identificirajte podvojeno proxyAddresses, userPrincipalName ali drugo vrednost atributa, ki povzroča napako. Določite tudi, kateri dve (ali več) predmetov sta udeleženi v sporu. Poročilo, ki ga ustvari Azure AD Connect Health za sinhronizacijo, vam lahko pomaga prepoznati dva predmeta.
    
2. Ugotovite, kateri predmet naj se nadaljuje s podvojeno vrednostjo in kateri predmet ne bi smel biti.
    
3. Odstranite podvojeno vrednost iz predmeta, ki ne bi smel imeti te vrednosti. Upoštevajte, da morate spremeniti mapo, v kateri je predmet nabavljan. V nekaterih primerih boste morda morali izbrisati enega od predmetov v sporu.
    
4. Če ste naredili spremembo v OGLASu na mestu uporabe, naj Azure AD poveže sinhronizacijo spremembe za napako, da se popravi.
    

