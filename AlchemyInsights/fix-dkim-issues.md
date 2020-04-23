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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717578"
---
# <a name="fix-dkim-setup-issues"></a>Odpravljanje težav z nastavitvijo DKIM

Če naletite na težave, ki omogočajo DKIM za vašo domeno po meri, uporabite naslednje korake:

- Večina težav z nastavitvijo DKIM je povezanih z nepravilnimi zapisi DNS. Preverite, ali je zapis DKIM CNAME (**ne** zapis txt) pravilno formatiran. Če želite več informacij, glejte to [temo](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Ko ustvarite ali posodobite zapise DKIM DNS v storitvi gostovanja DNS za vašo domeno (običajno je to registrar domene), počakajte, da se zapisi DNS razširijo.

- Če ne morete ustvariti zapisov DKIM DNS v skrbniškem središču, lahko \<zamenjate customdomain\> s svojo domeno po meri (na primer contoso.com) in zaženete ta ukaz v [PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
