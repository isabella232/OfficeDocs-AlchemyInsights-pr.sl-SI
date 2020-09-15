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
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691591"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Odpravljanje težav pri skupni rabi SharePointovih vsebin z zunanjimi Uporabniki

Prepričajte se, da je za vašo organizacijo vklopljena zunanja skupna raba:
  
1. Pojdite na [stran dodatki storitve &amp; v skrbniškem središču za Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)in kliknite **spletna mesta**.
    
2. Prepričajte se, da je nastavitev vklopljena na» vklopljeno «. Če je izbrana možnost» le obstoječi zunanji Uporabniki «, se prepričajte, da je zunanji uporabnik naveden v skrbniškem središču za Microsoft 365.
    
Prepričajte se, da je za spletno mesto vklopljena zunanja skupna raba. Za klasično zbirko mest:
  
1. V novem skrbniškem središču za SharePoint v levem podoknu kliknite **spletna mesta**.
    
2. Izberite mesto ali spletna mesta in na traku kliknite **Skupna raba**.
    
Za spletno mesto skupine, ki pripada skupini Microsoft 365 ali na spletnem mestu za komunikacijo:
  
- Te nove vrste mest imajo enako nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če nastavitev za celotno organizacijo omogoča skupno rabo datotek s povezavami, ki ne zahtevajo vpisa. V tem primeru spletna mesta omogočajo skupno rabo z novimi in obstoječimi zunanjimi Uporabniki, ki se vpišejo. Če želite spremeniti nastavitev za določena mesta, uporabite novo skrbniško središče za SharePoint ali PowerShell. [Več informacij](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Nastavitev zunanje skupne rabe za katero koli spletno mesto je lahko bolj restriktivna kot nastavitev za celotno organizacijo, ne pa tudi bolj zahtevna kot nastavitev za celotno organizacijo. 
  

