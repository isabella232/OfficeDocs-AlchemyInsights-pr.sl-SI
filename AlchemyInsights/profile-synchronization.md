---
title: Sinhronizacija profila
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801785"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kdaj se moj profil spremeni tako, da se sinhronizira z aplikacijo SharePointovega uporabniškega profila?

SharePoint online uporablja posel razporejevalnika za uvoz imenika Active Directory (uvoz oglasov) za uvoz uporabnikov in skupin v program uporabniškega profila. 
  
1. Uvoz oglasov sinhronizira spremembe iz trgovine imenika SharePoint online v aplikacijo uporabniškega profila. Te spremembe so obdelane v svežnjih.
    
2. Opravilo razporejevalnika se zažene, dokler se spremembe ne sinhronizirajo.
    
> [!NOTE]
> Čas trajanja posla je odvisen od števila sprememb, ki jih želite obdelati. Večje število sprememb traja dlje. Sporazum na ravni storitve (SLA) določa, da bo sprememba uporabnika v imeniku SharePoint Onlinea v programu uporabniškega profila prikazana v 24 urah. 
  
[Več informacij o sinhronizaciji uporabniškega profila v storitvi SharePoint online](https://go.microsoft.com/fwlink/?linkid=875671)
  

