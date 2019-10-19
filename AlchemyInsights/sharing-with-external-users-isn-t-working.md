---
title: Deljenje z zunanjimi uporabniki ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502247"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Odpravljanje težav pri skupni rabi SharePointove vsebine z zunanjimi Uporabniki

Prepričajte se, da je zunanja skupna raba vklopljena za vašo organizacijo:
  
1. Pojdite na [stran» &amp; dodatki za storitve «v skrbniškem središču za Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)in kliknite **mesta**.
    
2. Prepričajte se, da je nastavitev vklopljena. Če je izbrana možnost» samo obstoječi zunanji Uporabniki «, se prepričajte, da je zunanji uporabnik naveden v skrbniškem središču Microsoft 365.
    
Prepričajte se, da je zunanja skupna raba vklopljena za spletno mesto. Za klasično zbirko mest:
  
1. V novem skrbniškem središču SharePoint v levem podoknu kliknite **mesta**.
    
2. Izberite spletno mesto ali spletna mesta in na traku kliknite **Skupna raba**.
    
Za spletno mesto skupine, ki pripada skupini Office 365 ali na mestu za komunikacijo:
  
- Te nove vrste mest imajo enako nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če nastavitev za celotno organizacijo omogoča skupno rabo datotek s povezavami, ki ne zahtevajo prijave. V tem primeru spletna mesta omogočajo skupno rabo z novimi in obstoječimi zunanjimi Uporabniki, ki se vpisljajo. Če želite spremeniti nastavitev za določena mesta, uporabite nov SharePointov skrbniški center ali PowerShell. [Preberite več](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Nastavitev zunanje delitve za poljubno spletno mesto je lahko bolj omejevalna kot nastavitev za celotno organizacijo, vendar ne bolj permisivno kot nastavitev za celotno organizacijo. 
  

