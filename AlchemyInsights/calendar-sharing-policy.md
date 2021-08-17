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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091619"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Napaka pravilnika pri skupni rabi koledarja

1. Naredite nekaj od tega, kar je primerno za vašo situacijo:
    - Povezovalnik lahko Exchange Online z oddaljeno storitvijo PowerShell. Če želite več informacij, [Povezovalnik Exchange Online uporabo oddaljene lupine PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - V strežniku na mestu uporabe odprite ukazno lupino Exchange za upravljanje.
2. Določite pravilnik o skupni rabi, ki je dodeljen uporabniku. To naredite tako, da zaženete ta ukaz in zabeležite vrnjen pravilnik:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Posodobite pravilnik o skupni rabi za uporabnika. To naredite tako:
    - Odprite skrbniško Exchange za Office 365.
    - Kliknite **Organizacija** in nato dvokliknite pravilnik, ki je dodeljen uporabniku v razdelku **Posamezna skupna raba.** To je pravilnik, ki ste ga vrnili v 2. koraku.
    - Na strani Pravilo skupne rabe izberite raven skupne rabe koledarja, ki jo želite dovoliti v razdelku Določite, katere informacije želite dati **v skupno rabo;** kliknite **Shrani**.

Če želite več informacij, glejte: »Pravilnik ne dovoljuje podelitev dovoljenj na tej ravni za eno ali več prejemnikov« napake, ko uporabnik poskuša dati koledar [v skupno rabo.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
