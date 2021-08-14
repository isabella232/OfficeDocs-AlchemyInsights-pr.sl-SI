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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923660"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kdaj se moj profil spremeni SharePoint aplikacijo uporabniškega profila?

SharePoint V spletu uporablja posel časovnika za uvoz imenika Active Directory (AD Import) za uvoz uporabnikov in skupin v aplikacijo uporabniškega profila. 
  
1. Uvoz AD sinhronizira spremembe iz trgovine SharePoint Online Directory Store v aplikacijo uporabniškega profila. Te spremembe so obdelane v paketih.
    
2. Posel časovnika se izvaja, dokler spremembe niso sinhronizirane.
    
> [!NOTE]
> Čas, potreben za izvajanje posla, je odvisen od števila sprememb, ki jih je treba obdelati. Večje število sprememb traja dlje. Pogodba o ravni storitve določa, da se sprememba uporabnika v imeniku storitve SharePoint Online Directory v aplikaciji uporabniškega profila odraža v 24 urah. 
  
[Več informacij o sinhronizaciji uporabniških profilov v SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

