---
title: Ni mogoče dodati privzeti potek dela odobritve 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489519"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Ni mogoče dodati privzeti potek dela odobritve 2010

V zbirki mest Microsoft SharePoint, ne morete dodati globalno enkratno uporabo poteka dela (na primer "odobritev - SharePoint 2010") na seznam ali v knjižnico.
  
Če želite odpraviti to težavo, sledite tem korakom: 
  
1. Odprite spletni koren zbirke mest v SharePoint Designer 2013.
  
2. Pod **Stran predmetov**, izberite **potek dela**. 
  
3. V razdelku **Nova** **poteki dela** traku, izberite **Potek dela za vnovično uporabo**. 
  
4. **Ustvarite potek dela za vnovično uporabo** obrazcu, vnesite ime * **Repair2010***. Za **Tip platforme**, izberite **SharePointov potek dela 2010**, in izberite **OK**. 
  
5. V razdelku **shranjevanje** **potek dela** traku izberite **objavi**. 
  
6. V razdelku **upravljanje** **poteka dela** traku izberite **Objavi globalno**. V pogovornem oknu potrditve, ki se prikaže, izberite **OK**. 
  
7. V spletnem brskalniku, poiščite korenski spletni strani zbirke mest in nato dostopate do **Nastavitev mesta** \> **Funkcij zbirke mest**. Nato, zatik zunanja oblika **potekov dela** : 
  
· Če zunanja oblika je *Activated* , kliknite **Deactivate,** in nato kliknite **Aktiviraj**. 
  
· Če funkcija je *deaktivirani* , kliknite **Aktiviraj**. 
  
Za več informacij si oglejte [članek](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

