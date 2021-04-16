---
title: Upokojitev podedovanih orodij za e-odkrivanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798565"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Upokojitev podedovanih orodij za e-odkrivanje

Zaradi nove in izboljšane funkcije e-odkrivanja v središču za skladnost s predpisi storitve Microsoft 365 bodo v prihodnjih mesecih ukinjena ta podedovana orodja za e-odkrivanje in ukazni ukazi:

- [E-odkrivanje na mestu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [in zadržanja na mestu v](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) skrbniškem središču za Exchange.

- Ukazi »cmdlet« lupine PowerShell za Exchange Online, In-Place e-odkrivanje in In-Place zadržanja. (Te ukaze »cmdlet« je mogoče skupaj določiti kot ukaze »cmdlet« *-MailboxSearch.) To vključuje te ukaze »cmdlet«:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Iskanje po začetnem nabiralniku](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Ukaz [»cmdlet« za iskanje](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v nabiralniku v lupini PowerShell za Exchange Online.
- Te operacije v VMESNIKU API za Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časovnica za upokojitev:**
- **1. julij 2020** Ne morete več ustvarjati novih iskan in zadržanj, lahko pa izvajate, urejate in brišete obstoječa iskanja na lastno odgovornost. Microsoftova podpora ne podpira več In-Place zadržanj e-& v EAC.
    
- **1. oktober 2020** In-Place funkcijo e-odkrivanja & Zadržanja bodo v EAC postavljena v način samo za branje, tako da lahko odstranite le obstoječa iskanja in zadržanja.

**Če želite več informacij, glejte:**

 - [Selitev podedovanih iskancev e-odkrivanja in zadržanja v središče za skladnost s predpisi storitve Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Umik podedovanih orodij za e-odkrivanje](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Pogosta vprašanja o In-Place e-odkrivanju in In-Place zadržanjih](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



