---
title: 1336 RecoverableItems mapa je polna
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312393"
---
# <a name="the-recoverable-items-folder-is-full"></a>«Mapa »Obnovljivo «je poln

Za nabiralnikov Exchange Online v Office 365, privzeto omejitev velikosti shrambe za mapo »Obnovljivo« je 30 GB. Omejitev velikosti shrambe za mapo »Obnovljivo« se samodejno poveča na 100 GB, če nabiralnik je postavljena na čakanje, eDiscovery drži, ali je dodeljen pravilnik o hranjenju z Office 365.
  
Ko mapo »Obnovljivo «doseže omejitev velikosti shrambe, nabiralnik funkcionalnost vpliva na naslednje načine:
  
- Uporabnik ne more izbrisati elemente iz nabiralnika.
    
- Pomočnik za upravljane mape ne morete izbrisati elementov glede na oznako za hranjenje ali nastavitve za upravljane mape.
    
- Za nabiralnike, ki imajo omogočeno obnovitvijo posamezen element ali so postavljena na čakanje, kopijo na napišite strani zaščitnega postopka ne more vzdrževati različice elementov, ki jih bo uporabnik.
    
- Za nabiralnike, ki so nabiralnik revizijo omogočenim pisanjem dnevnika, vnose v dnevnik nadzora ni nabiralnik lahko shranite v revizije podmapo v mapi »obnovljivo« .
    
Za nabiralnike, ki niso na čakanju, administratorji lahko uporabite na `Search-Mailbox -SearchDumpsterOnly -DeleteContent` v Exchange Online PowerShell za brisanje elementov v mapi »obnovljivo« . Če želite več informacij, glejte te teme: 
  
- [Iskanje in brisanje sporočil](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Za nabiralnike, ki so na čakanju, administratorji morali odstraniti zadržanja, preden se lahko izbrisano iz mape »Obnovljivo« . Če želite več informacij, glejte [brisanje elementov v obnovljivo mapo oblaku nabiralnikov na imajo](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Da bi preprečili mape »Obnovljivo« od postane poln, lahko administratorji poveča omejitev velikosti shrambe za obnovljivo mapo za nabiralnike v strežniku imajo in nastavite pravilnika o hranjenju za nabiralnik, ki premakne elemente iz mape »Obnovljivo« v uporabnikovem Arhiv nabiralnik. Glej, [povečanje obnovljivo imajo količinske omejitve za nabiralnike v strežniku](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

