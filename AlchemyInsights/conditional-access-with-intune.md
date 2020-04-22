---
title: Pogojni dostop z InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706037"
---
# <a name="conditional-access-with-intune"></a>Pogojni dostop z InTune

Uporaba **pogojnega dostopa** z InTune zahteva 3 korake: 
  
- Ustvarite **pravilnik pogojnega dostopa** , ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolniti za dostop do teh virov. Naprava mora biti na primer skladna pred dostopom do e-pošte podjetja. 
    
- Ustvarite **pravilnik o skladnosti** , če želite določiti nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za združljivo. Naprava mora imeti na primer PIN vsaj 6 števk, preden se šteje za skladno. 
    
- Zagotavljanje, da **Pravilniki o skladnosti** in pravilniki o **pogojnem dostopu** ciljajo na želene skupine uporabnikov. To lahko zahteva ustvarjanje določenih skupin uporabnikov v storitvi Azure Active Directory. 
    
Preberite več:
  
- [Najboljši postopki za pogojni dostop](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Uvod v pogojni dostop](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

