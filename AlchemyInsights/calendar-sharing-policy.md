---
title: 618 koledar črepina zvitost
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373015"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Napaka pravilnika pri skupni rabi koledarja

1. Naredite nekaj od tega, kot je primerno za vaše stanje:
    - Vzpostavite povezavo s storitvijo Exchange Online z oddaljenim PowerShell. Če želite več informacij, glejte [Vzpostavljanje povezave s storitvijo Exchange Online z oddaljenim PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - V krajevnem strežniku odprite lupino za upravljanje Exchangeevega.
2. Določite pravilnik o delitvi, ki je dodeljen uporabniku. Če želite to narediti, zaženite ta ukaz in upoštevajte, da se je pravilnik vrnil:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Posodobite pravilnik o skupni rabi za uporabnika. Če želite to narediti, sledite tem korakom:
    - Odprite skrbniški center Exchange.
    - Kliknite **organizacija**in nato dvokliknite pravilnik, ki je dodeljen uporabniku v okviru **posamezne skupne rabe**. To je pravilnik, ki je bil vrnjen v koraku 2.
    - Na strani pravilo delitve izberite raven skupne rabe koledarja, ki jo želite dovoliti v razdelku **določanje, katere informacije želite deliti z drugimi**; kliknite **Shrani**.

Če želite več informacij, glejte: [» pravilnik ne dovoljuje dodelitve dovoljenj na tej ravni enemu ali več napaki prejemnika «, ko uporabnik poskuša deliti koledar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
