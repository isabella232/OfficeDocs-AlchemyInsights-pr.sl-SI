---
title: Upokojitev Legacy orodja e-odkrivanja
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650584"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Upokojitev Legacy orodja e-odkrivanja

Zaradi nove in izboljšane funkcionalnosti e-odkrivanja v Microsoftovem 365 centru za skladnost bodo v naslednjih mesecih upokojeni naslednji podedovani orodji e-discovery in Commandlets:

- In [-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) in [v mestu ima](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v skrbniškem središču Exchange.

- Cmdlets za Exchange Online PowerShell, ki podpirajo e-odkrivanje in-Place v mestu. (Ti ukazi» cmdlet «so skupno označeni kot» cmdlet «-MailboxSearch.) To vključuje naslednje ukaze» cmdlet «:

    - [Novo-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Zaustavitev-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Ukaz» cmdlet «za [Iskanje-nabiralnik](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v PowerShell Exchange Online.
- Naslednje operacije v API-ju storitve Exchange Web Services:
    - [Getsearchablenabiralniki](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonnabiralniki](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonnabiralniki](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Napredno eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časovna premica za upokojitev**:
- 1. april 2020: ne boste mogli ustvariti novih iskanj in zadržanj, vendar lahko še vedno zaženete, urejate in izbrišete obstoječa iskanja na lastno odgovornost. Microsoftova podpora ne bo več podpirala in-Place eDiscovery & zadržki v EAC.

- 1. julij 2020: funkcija eDiscovery & na mestu delovanja v EAC bo postavljena v način samo za branje. To pomeni, da boste lahko odstranili obstoječa iskanja in zadržki.

**Za več informacij glejte**:

 - [Selitev podedovanih iskanj e-odkrivanja in skladišč v središče za skladnost z Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Upokojitev starejših orodij e-odkrivanja](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Pogosta vprašanja o eDiscovery v mestu in kraju](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



