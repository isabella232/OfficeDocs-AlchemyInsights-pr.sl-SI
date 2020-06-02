---
title: Odpravljanje težav z nastavitvijo DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506790"
---
# <a name="fix-dkim-setup-issues"></a>Odpravljanje težav z nastavitvijo DKIM

Če naletite na težave, ki omogočajo DKIM za vašo domeno po meri, uporabite naslednje korake:

- Večina težav z nastavitvijo DKIM je povezanih z nepravilnimi zapisi DNS. Preverite, ali je zapis DKIM CNAME (**ne** zapis txt) pravilno formatiran. Če želite več informacij, glejte to [temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Ko ustvarite ali posodobite zapise DKIM DNS v storitvi gostovanja DNS za vašo domeno (običajno je to registrar domene), počakajte, da se zapisi DNS razširijo.

- Če v skrbniškem središču ne morete ustvariti zapisov DKIM DNS, lahko zamenjate \<CustomDomain\> z domeno po meri (na primer contoso.com) in zaženete ta ukaz v [PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
