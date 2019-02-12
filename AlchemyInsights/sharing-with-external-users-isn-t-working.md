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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900904"
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
  

