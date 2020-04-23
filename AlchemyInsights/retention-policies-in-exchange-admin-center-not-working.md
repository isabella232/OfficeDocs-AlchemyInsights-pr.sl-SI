---
title: Pravilniki o hranjenju v skrbniškem središču za Exchange ne delujejo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742449"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravilniki o hranjenju v skrbniškem središču Exchange

 **Vprašanje:** Na novo ustvarjene ali posodobljene pravilnike o hranjenju v skrbniškem središču za Exchange se ne uporabljajo za nabiralnike ali artikle, ki niso premaknjeni v arhivski nabiralnik ali izbrisani. 
  
 **Temeljni vzroki:**
  
- To je morda zato, ker **pomočnik za upravljane mape** ni obdelal uporabnikovega nabiralnika. Pomočnik za upravljane mape poskuša obdelati vsak nabiralnik v organizaciji v oblaku vsakih sedem dni. Če spremenite oznako za hranjenje ali v nabiralnik uporabite drug pravilnik o hranjenju, lahko počakate, da postopek pomoči za upravljano mapo obdela nabiralnik, lahko pa zaženete ukaz» cmdlet «Start-ManagedFolderAssistant, da zaženete pomočnika za upravljane mape, da obdela določen nabiralnik. Zagon tega ukaza» cmdlet «je uporaben za preskušanje ali odpravljanje težav z nastavitvami pravilnika o hranjenju ali oznake za hranjenje. Če želite več informacij, preberite [zagon pomočnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rešitev:** Zaženite ta ukaz, da zaženete pomočnika za upravljane mape za določen nabiralnik:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To se lahko zgodi tudi, če je bil v nabiralniku **omogočen** **RetentionHold** . Če je bil nabiralnik postavljen na RetentionHold, pravilnik o hranjenju v nabiralniku v tem času ne bo obdelan. Za več informacij o nastavitvi RetentionHold glejte: [zadržanje hranjenja nabiralnika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rešitev:**
    
  - Preverite stanje nastavitve RetentionHold v določenem nabiralniku v [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Zaženite ta ukaz, da **onemogočite** RetentionHold v določenem nabiralniku:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Zdaj znova zaženite pomočnika za upravljane mape:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.
 
Če želite več informacij o pravilnikih hranjenja v skrbniškem središču za Exchange, glejte:
- [Oznake za hranjenje in pravilniki o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodajanje ali odstranjevanje oznak za hranjenje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako prepoznati vrsto zadržanja, danega v nabiralnik](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
