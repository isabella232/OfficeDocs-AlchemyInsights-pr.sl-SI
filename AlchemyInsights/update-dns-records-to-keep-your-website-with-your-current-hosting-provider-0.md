---
title: Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja
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
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312408"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Posodobiti zapise DNS, da vaše spletne strani s svojega trenutnega ponudnika gostovanja

1. Na [področje](https://portal.office.com/adminportal/home#/Domains) strani, domen, na seznamu izberite domeno uporabljate za vašo spletno stran, in nato izberite **nastavitve DNS** v podokno upravljanje. 
    
2. **+ Nov zapis po meri** in vnesite naslednje: 
    
  - Za **DNS vrsta** vnesite: **(naslov)**
    
  - **Ime gostitelja ali Alias**, vnesite naslednje:**@**
    
  - Za **IP naslov**, vnesite statični naslov IP za vašo spletno stran, kjer je trenutno gosti (npr. 172.16.140.1). 
    
    To mora biti *statični* naslov IP za spletno stran, ne *dinamični* IP naslov. Preveriti s mesto, kjer vašo spletno stran gostuje prepričati se lahko dobite statični naslov IP za javne spletne strani. 
    
3. Izberite **Shrani**. 
    
Poleg tega lahko ustvarite zapis CNAME za pomoč uporabniki našli vašo spletno stran.
  
1. **+ Nov zapis po meri** in vnesite naslednje: 
    
  - Za **DNS vrsta** vnesite: **CNAME (Alias)**
    
  - **Ime gostitelja ali Alias**, vnesite naslednje: **www**
    
  - Za **točki naslov**, vnesite ime domene (FQDN) za vašo spletno stran (na primer contoso.com). 
    
2. Izberite **Shrani**. 
    

