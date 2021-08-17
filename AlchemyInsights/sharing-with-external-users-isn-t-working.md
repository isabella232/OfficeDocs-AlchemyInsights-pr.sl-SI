---
title: Skupna raba z zunanjimi uporabniki ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304385"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Odpravljanje težav s skupno SharePoint vsebine z zunanjimi uporabniki

Preverite, ali je zunanja skupna raba za vašo organizacijo vklopljena:
  
1. Pojdite na [stran z dodatki storitve v Skrbniško središče za Microsoft 365 &amp; in](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)kliknite **Mesta.**
    
2. Prepričajte se, da je nastavitev vklopljena na »Vklopljeno«. Če je izbrana možnost »Samo obstoječi zunanji uporabniki«, preverite, ali je zunanji uporabnik naveden v Skrbniško središče za Microsoft 365.
    
Preverite, ali je zunanja skupna raba za mesto vklopljena. Za klasično zbirko mest:
  
1. V novem skrbniškem SharePoint v levem podoknu kliknite **Mesta.**
    
2. Izberite mesto ali spletna mesta in na traku kliknite Skupna **raba.**
    
Za spletno mesto skupine, ki pripada Microsoft 365 skupini ali spletnemu mestu za komunikacijo:
  
- Te nove vrste spletnih mest imajo enako nastavitev skupne rabe kot za celotno organizacijo, razen če nastavitev za celotno organizacijo omogoča skupno rabo datotek s povezavami, ki ne zahtevajo vpisa. V tem primeru mesta omogočajo skupno rabo z novimi in obstoječimi zunanjimi uporabniki, ki se vpišejo. Če želite spremeniti nastavitev za določena mesta, uporabite novo skrbniško središče SharePoint ali PowerShell. [Več informacij](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Opomba:** Nastavitev zunanje skupne rabe za katero koli spletno mesto je lahko bolj omejujoča kot nastavitev za celotno organizacijo, vendar ne bolj jo je mogoče sprejemati kot nastavitev na ravni organizacije. 
  

