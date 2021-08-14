---
title: Odpravljanje težav z nastavitvijo DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945947"
---
# <a name="fix-dkim-setup-issues"></a>Odpravljanje težav z nastavitvijo DKIM

Če pride do težav pri omogočanju kontrolnika DKIM za domeno po meri, sledite tem korakom:

- Večina težav z nastavitvijo DKIM je povezanih z nepravilnimi zapisi DNS. Preverite, ali je zapis DKIM CNAME **(ne** zapis TXT) pravilno oblikovan. Če želite več informacij, glejte to [temo.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Ko ustvarite ali posodobite zapise DNS DKIM v storitvi gostovanja DNS za svojo domeno (običajno je to registrator domene), počakajte, da se zapisi DNS razširijo.

- Če ne morete ustvariti zapisov DKIM DNS v skrbniškem središču, lahko zamenjate z domeno po meri (na primer contoso.com) in zaženete ta ukaz v \<CustomDomain\> [storitvi Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
