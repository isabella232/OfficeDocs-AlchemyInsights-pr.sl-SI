---
title: Pogojni dostop z InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505010"
---
# <a name="conditional-access-with-intune"></a>Pogojni dostop z InTune

Uporaba **pogojnega dostopa** z InTune zahteva 3 korake: 
  
- Ustvarite **pravilnik pogojnega dostopa** , ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolniti za dostop do teh virov. Naprava mora biti na primer skladna pred dostopom do e-pošte podjetja. 
    
- Ustvarite **pravilnik o skladnosti** , če želite določiti nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za združljivo. Naprava mora imeti na primer PIN vsaj 6 števk, preden se šteje za skladno. 
    
- Zagotavljanje, da **Pravilniki o skladnosti** in pravilniki o **pogojnem dostopu** ciljajo na želene skupine uporabnikov. To lahko zahteva ustvarjanje določenih skupin uporabnikov v storitvi Azure Active Directory. 
    
Preberite več:
  
- [Najboljši postopki za pogojni dostop](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Uvod v pogojni dostop](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

