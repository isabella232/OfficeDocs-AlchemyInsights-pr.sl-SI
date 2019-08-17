---
title: Pravilniki o hranjenju v Exchange Admin Center ne deluje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444824"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravilniki o hranjenju v skrbniškem središču za izmenjavo

 **Izdaje:** Na novo ustvarjeno ali posodobljeno zadrževanja v skrbniškem središču za izmenjavo ne veljajo za nabiralnike ali artikli ne premesti arhivskega nabiralnika ali izbrisati. 
  
 **Vzrokov:**
  
- To se lahko ker je **Pomočnik upravljane mape** ni predelana uporabnikovega nabiralnika. Pomočnik za upravljane mape Windows poskusi obdelati vse nabiralnike v organizaciji oblaku enkrat vsakih sedem dni. Če spremenite oznako za hranjenje ali uporabljajo pravilnik z nabiralnikom, lahko počakate, dokler uspelo mape pomagajo obdela nabiralnik, ali lahko zaženete ukaz cmdlet Start-ManagedFolderAssistant začeti pomočnik za upravljane mape za obdelavo določenega nabiralnik. Teče ta ukaz »cmdlet« je namenjen preskušanju ali odpravljanju pravilnika o hranjenju ali tag nastavitve hranjenja. Če želite več informacij, obiščite [prost dostop pomočnik za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Raztopina:** Prost dostop sledeč zapoved v začetek pomočnik za upravljane mape za določen nabiralnik:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Pojavi se to lahko tudi, če **RetentionHold** je bila **omogočena** v nabiralniku. Če nabiralnik je postavljena na RetentionHold, s pravilnikom o hranjenju, v nabiralniku ne bo obdelan v tem času. Za več informacije na RetentionHold nastavitev glej: [Nabiralnik hranjenja čakanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rešitev:**
    
  - Preverite stanje RetentionHold nastavitev na določen nabiralnik v [EKSO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Prost dostop sledeč zapoved v **onesposobiti** RetentionHold na določen naslov:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Zdaj, znova zaženite upravljane mape pomočnik:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Opomba:** Če nabiralnik je manjši od 10 MB, pomočnik za upravljane mape bo samodejno obdela nabiralnik.
 
Za več informacij o pravilniki o hranjenju v skrbniškem središču Exchange, glejte:
- [Oznake za hranjenje in pravilniki o hranjenju](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Uporablja pravilnik o hranjenju za nabiralnike](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodajanje ali odstranitev oznake za hranjenje](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako ugotoviti vrsto drži dano na nabiralnik](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
