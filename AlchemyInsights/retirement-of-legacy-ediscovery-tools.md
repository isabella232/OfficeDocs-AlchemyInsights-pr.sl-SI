---
title: Upokojitev podedovanih E-odkrivanje orodij
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902636"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Upokojitev podedovanih E-odkrivanje orodij

Kot rezultat nove in izboljšane funkcije E-odkrivanje v središču za skladnost s predpisi Microsoft 365 se bodo v prihodnjih mesecih umaknila naslednja podedovana E-odkrivanje orodja in ukazov:

- [Na mestu e-odkrivanje](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) in [na](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) mestu uporabe v skrbniškem središču za Exchange.

- Ukazi» cmdlet «za Exchange Online, ki podpirajo na mestu E-odkrivanje in na mestu uporabe. (Ti ukazi» cmdlet «so skupaj opredeljeni kot *-MailboxSearch ukazi» cmdlet «.) To vključuje te ukaze» cmdlet «:

    - [Novo-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Zaustavitev-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Ukaz» cmdlet « [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v storitvi Exchange Online PowerShell.
- Te operacije v API-jih storitve Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Napredno E-odkrivanje v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časovnica za upokojitev**:
- **1. julij 2020** Ne morete več ustvarjati novih iskanj in jih prihraniti, lahko pa zaganjate, urejate in brišete obstoječa iskanja na lastno odgovornost. Microsoftova podpora ni več podprta na mestu E-odkrivanje, & ima v programu EAC.
    
- **1. oktober 2020** Na mestu E-odkrivanje & funkcija ima funkcionalnost v programu EAC, ki bo v načinu samo za branje, zato lahko odstranite le obstoječa iskanja in zadržanje.

Če **želite več informacij, glejte**:

 - [Selitev podedovanih E-odkrivanje iskanj in zadržanje v središču za skladnost s predpisi Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Upokojitev podedovanih E-odkrivanje orodij](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Pogosta vprašanja o E-odkrivanje na mestu uporabe in na mestu uporabe](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



