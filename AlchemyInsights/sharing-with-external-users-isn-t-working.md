---
title: Delitev z zunanjim uporabnikom ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312744"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Odpravite težave, delitev SharePointovo vsebino z zunanjim uporabnikom

Poskrbite, zunanja delitev vklopljena v organizaciji:
  
1. Pojdi na [storitev &amp; dodatki stran v skrbniškem središču za Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), in kliknite **mesta**.
    
2. Poskrbite, da nastavitev je obrnil k "O." Če je izbrana "Le obstoječe zunanje uporabnike", se prepričajte, zunanjo uporabnik je prisluškovati v skrbniškem središču za Office 365.
    
Poskrbite, zunanja delitev vklopljen za mesto. Klasična mest:
  
1. V klasičnih SharePoint admin center, v levem podoknu kliknite **zbirke mest**.
    
2. Izberite kraj ali kraje, in na traku kliknite **Skupna raba**.
    
Mesto ekipa, ki pripada skupini Office 365, ali mesto komunikacije:
  
- Te nove vrste mesta imajo isto nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če celotno organizacijo nastavitev omogoča izmenjavo datotek prek povezave, ki ne zahtevajo vpis. V tem primeru mesta omogočajo izmenjavo z novim in obstoječim zunanjim uporabnikom, ki vpisati. Spremeniti nastavitev za določene strani, uporabite novo SharePoint admin center (predogled) ali PowerShell. [Več](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Nastavitev za zunanji skupno rabo za vse strani lahko bolj omejujoča kot nastavitev celotno organizacijo, vendar ne manj zahtevnimi kot nastavitev za celotno organizacijo. 
  

