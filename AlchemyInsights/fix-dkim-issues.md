---
title: Popraviti DKIM nastavljanjem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765417"
---
# <a name="fix-dkim-setup-issues"></a>Popraviti DKIM nastavljanjem

Če imate vprašanja, ki omogočajo DKIM za domeno po meri, sledite naslednjim korakom:

- Večina DKIM namestitev vprašanja so povezana z napačne zapise DNS. Preverite, ali zapis DKIM CNAME (**ne** zapis TXT) pravilno oblikovana. Če želite več informacij, glejte to [temo](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Ko ustvarite ali posodobiti vaše DKIM DNS zapisov na DNS sovražen usluga za domeno (praviloma svojega registratorja domene), čakati na zapise DNS, da širi.

- Če ne morete ustvariti DKIM DNS zapisov v skrbniškem središču, lahko zamenjate \<CustomDomain\> z domeno po meri (na primer contoso.com) in zaženite ta ukaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
