---
title: Pravilniki o hranjenju v skrbniškem središču za Exchange ne delujejo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740526"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravilniki o hranjenju v skrbniškem središču za Exchange

Če želite, da zaženemo avtomatizirane kontrole za spodaj navedene nastavitve, izberite gumb» Vrni «< na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s pravilniki o hranjenju.

 **Težava:** Novo ustvarjene ali posodobljene pravilnike o hranjenju v skrbniškem središču za Exchange se ne uporabljajo za nabiralnike ali elemente, ki niso premaknjeni v arhivski nabiralnik ali izbrisani. 
  
 **Vzroki vzrokov:**
  
- To je morda zato, ker **pomočnik za upravljane mape** ni obdelal nabiralnika uporabnika. Pomočnik za upravljane mape poskuša obdelati vse nabiralnike v organizaciji v oblaku vsakih sedem dni. Če spremenite oznako za hranjenje ali v nabiralnik uporabite drug pravilnik o hranjenju, lahko počakate, da upravljana mapa pomaga pri obdelavi nabiralnika, lahko pa zaženete ukaz» cmdlet «Start-ManagedFolderAssistant, da zaženete pomočnika za upravljane mape za obdelavo določenega nabiralnika. Zagon tega ukaza» cmdlet «je uporaben za preskušanje ali odpravljanje težav s pravilnikom o hranjenju ali postavljanjem oznak za hranjenje. Če želite več informacij, obiščite spletno mesto [Zaženi pomočnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rešitev:** Zaženite ta ukaz, da zaženete pomočnika za upravljane mape za določen nabiralnik:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Do tega lahko pride tudi, če je v nabiralniku **omogočeno** **RetentionHold** . Če je bil nabiralnik nameščen v RetentionHold, se pravilnik o hranjenju v nabiralniku v tem času ne bo obdelal. Če želite več namestitvi v nastavitvi RetentionHold, glejte: zadržanje [nabiralnika](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rešitev**
    
  - Preverite stanje nastavitve RetentionHold za določen nabiralnik v storitvi [ekso PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Zaženite ta ukaz, če želite **onemogočiti** RetentionHold v določenem nabiralniku:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Zdaj znova zaženite pomočnika za upravljane mape:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Opomba:** Če je nabiralnik manjši od 10 MB, pomočnik za upravljane mape ne bo samodejno obdelal nabiralnika.
 
Če želite več informacij o pravilnikih o hranjenju v skrbniškem središču za Exchange, glejte:
- [Oznake hranjenja in pravilniki o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodajanje ali odstranjevanje oznak za hranjenje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako prepoznati vrsto zadržanja, ki je nameščena v nabiralniku](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
