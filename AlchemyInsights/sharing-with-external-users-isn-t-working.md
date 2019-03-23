---
title: Delitev z zunanjim uporabnikom ne deluje
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
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753442"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Odpravite težave, delitev SharePointovo vsebino z zunanjim uporabnikom

Poskrbite, zunanja delitev vklopljena v organizaciji:
  
1. Pojdi na [storitev &amp; dodatki stran v Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), in kliknite **mesta**.
    
2. Poskrbite, da nastavitev je obrnil k "O." Če je izbrana "Le obstoječe zunanje uporabnike", poskrbite, da zunanjo uporabnik iz Microsoft 365 admin center.
    
Poskrbite, zunanja delitev vklopljen za mesto. Klasična mest:
  
1. V klasičnih SharePoint admin center, v levem podoknu kliknite **zbirke mest**.
    
2. Izberite kraj ali kraje, in na traku kliknite **Skupna raba**.
    
Mesto ekipa, ki pripada skupini Office 365, ali mesto komunikacije:
  
- Te nove vrste mesta imajo isto nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če celotno organizacijo nastavitev omogoča izmenjavo datotek prek povezave, ki ne zahtevajo vpis. V tem primeru mesta omogočajo izmenjavo z novim in obstoječim zunanjim uporabnikom, ki vpisati. Spremeniti nastavitev za določene strani, uporabite novo SharePoint admin center (predogled) ali PowerShell. [Več](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Nastavitev za zunanji skupno rabo za vse strani lahko bolj omejujoča kot nastavitev celotno organizacijo, vendar ne manj zahtevnimi kot nastavitev za celotno organizacijo. 
  

