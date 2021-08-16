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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002136"
---
# <a name="error-attributevaluemustbeunique"></a>Napaka: AttributeValueMustBeUnique

Najpogostejši razlog za napako AttributeValueMustBeUnique sta dva predmeta z različnima atributoma SourceAnchor (immutableId) in proxyAddresses in/ali UserPrincipalName. Če želite odpraviti napako AttributeValueMustBeUnique:
  
1. Identificirajte podvojene vrednosti proxyAddresses, userPrincipalName ali drugo vrednost atributa, ki povzroča napako. Določite tudi, kateri predmeti (ali več) so vključeni v spor. V poročilu, ki ga ustvari storitev Azure AD Povezovalnik Health za sinhronizacijo, boste lažje prepoznali dva predmeta.
    
2. Določite, kateri predmet bo še naprej imel podvojeno vrednost in kateri predmet ne sme biti.
    
3. Odstranite podvojeno vrednost iz predmeta, ki bi moral IMETI to vrednost. Upoštevajte, da morate spremeniti imenik, iz katerem je vir predmeta. V nekaterih primerih boste morda morali izbrisati enega od predmetov v sporu.
    
4. Če ste naredili spremembe v imeniku AD na mestu uporabe, pustite, da imenik Azure AD Povezovalnik spremembo napake, da jo popravite.
    

