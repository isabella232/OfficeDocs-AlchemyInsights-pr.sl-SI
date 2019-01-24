---
title: E-poštnih sporočil premakniti arhivskega nabiralnika
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489987"
---
Težave, arhiviranje elementov v arhivski nabiralnik. Poskrbite, da boste izvedli naslednje korake:
  
1. Potrditev, da je bila omogočena **Arhiv nabiralnik** . V nasprotnem primeru, sledite korakom v [tem članku](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) za omogočanje arhivskega nabiralnika. 
    
2. V središču Admin Exchange izberite **Oznake za hranjenje** pod **Vodstvom, skladnost**, ustvariti **oznako za hranjenje** z dejanjem **premaknete Arhiv** , ki vsebuje želeno **Hranjenja**.
    
3. V skrbniškem središču Exchange, izberite **Pravilniki o hranjenju**, ustvarite **Pravilnik o hranjenju** in dodajte vaše **preseliti Arhiv** oznako za hranjenje politike. 
    
4. Za posebne uporabnikovega nabiralnika [dodelite pravilnik o hranjenju](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) . Istega pravilnika veljajo na **primarnega** in **arhivskega** nabiralnika. 
    
Uporabnikovega nabiralnika se pravilnik arhiviranja, ki ga želite premikati elemente v arhivski nabiralnik. Je potrebno za vsiljevanje uspelo mapo pomočnika (MFA) teči ter uveljavil nove nastavitve uporabnikovega nabiralnika. Zaženite ta ukaz, medtem ko [povezati EKSO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) začeti pomočnik za upravljane mape za določen nabiralnik: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Želite več informacij o vzpostavitvi pravilnik arhiviranja, glejte [Nastavitev Arhiv in izbris pravilnika za nabiralnike](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

