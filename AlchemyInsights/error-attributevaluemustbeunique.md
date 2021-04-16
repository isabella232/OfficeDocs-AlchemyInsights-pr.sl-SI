---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813776"
---
# <a name="error-attributevaluemustbeunique"></a>Napaka: AttributeValueMustBeUnique

Najpogostejši razlog za napako AttributeValueMustBeUnique sta dva predmeta z različnima atributoma SourceAnchor (immutableId) in proxyAddresses in/ali UserPrincipalName. Če želite odpraviti napako AttributeValueMustBeUnique:
  
1. Identificirajte podvojene vrednosti proxyAddresses, userPrincipalName ali drugo vrednost atributa, ki povzroča napako. Določite tudi, kateri predmeti (ali več) so vključeni v spor. S poročilom, ki ga ustvari Azure AD Connect Health za sinhronizacijo, boste lažje prepoznali dva predmeta.
    
2. Določite, kateri predmet bo še naprej imel podvojeno vrednost in kateri predmet ne sme biti.
    
3. Odstranite podvojeno vrednost iz predmeta, ki bi moral IMETI to vrednost. Upoštevajte, da morate spremeniti imenik, iz katerem je vir predmeta. V nekaterih primerih boste morda morali izbrisati enega od predmetov v sporu.
    
4. Če ste naredili spremembe v imeniku AD na mestu uporabe, pustite, da Azure AD Connect sinhronizira spremembo napake, da bo odpravljena.
    

