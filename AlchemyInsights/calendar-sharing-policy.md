---
title: Pravilnik o skupni rabi koledarja 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684246"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Napaka pravilnika pri skupni rabi koledarja

1. Naredite nekaj od tega, odvisno od tega, ali je to primerno za vaše stanje:
    - Vzpostavljanje povezave s storitvijo Exchange Online z uporabo oddaljenega PowerShella. Če želite več informacij, glejte [Vzpostavljanje povezave s storitvijo Exchange Online z oddaljeno lupino PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - V strežniku na mestu uporabe odprite lupino za upravljanje Exchangea.
2. Določite pravilnik o skupni rabi, ki je dodeljen uporabniku. Če želite to narediti, zaženite ta ukaz in zapomnite, da je pravilnik vrnjen:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Posodobite pravilnik o skupni rabi za uporabnika. Če želite to narediti, upoštevajte ta navodila:
    - Odprite skrbniško središče za Exchange.
    - Kliknite **organizacija**in nato dvokliknite pravilnik, ki je uporabniku dodeljen v okviru **posamezne skupne rabe**. To je pravilnik, ki je bil vrnjen v koraku 2.
    - Na strani pravilo skupne rabe izberite raven skupne rabe koledarja, ki jo želite omogočiti v razdelku **določanje podatkov, ki jih želite dati v skupno rabo**; kliknite **Shrani**.

Če želite več informacij, si oglejte: [» pravilnik ne dovoljuje dodeljevanja dovoljenj na tej ravni za enega ali več uporabnikov «napak, ko uporabnik poskuša dati koledar v skupno rabo](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
