---
title: Sinhronizacija profila
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768129"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kdaj se moj profil spremeni v sinhronizacijo s programom SharePoint User profile?

SharePoint online uporablja posel razporejevalnika uvoza imenika Active Directory (uvoz oglasa) za uvoz uporabnikov in skupin v aplikacijo uporabniškega profila. 
  
1. Uvoz oglasov sinhronizira spremembe iz trgovine SharePoint online Directory v aplikacijo uporabniškega profila. Te spremembe se obdelujejo v serijah.
    
2. Posel razporejevalnika se zažene, dokler se spremembe ne sinhronizirajo.
    
> [!NOTE]
> Čas, potreben za zagon posla, je odvisen od števila sprememb procesa. Veliko število sprememb traja dlje. Pogodba o ravni storitve (SLA) določa, da se bo sprememba uporabnika v SharePointovem spletnem imeniku odražala v aplikaciji uporabniškega profila v 24 urah. 
  
[Več informacij o sinhronizaciji uporabniških profilov v spletnem mestu SharePoint online](https://go.microsoft.com/fwlink/?linkid=875671)
  

