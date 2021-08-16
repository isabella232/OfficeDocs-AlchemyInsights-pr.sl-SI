---
title: Odpravljanje težav z dostavo e-pošte v javnih mapah z omogočeno e-pošto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068828"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Odpravljanje težav z dostavo e-pošte v javnih mapah z omogočeno e-pošto

Če zunanji pošiljatelji ne morejo pošiljati sporočil v javne mape z omogočeno e-pošto in pošiljatelji prejmejo napako: ni bilo mogoče najti **(550 5.4.1)**, preverite, ali je e-poštna domena za javno mapo konfigurirana kot notranja relejna domena in ne kot avtoritativna domena:

1. Odprite [skrbniško Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Pojdite na **Domene s** \> **sprejetim tokom pošte**, izberite sprejeto domeno in nato kliknite **Uredi**.

3. Če je na strani z lastnostmi, ki se odpre, vrsta  domene nastavljena na **Avtoritativno,** spremenite vrednost na Notranje posredovanje in kliknite **Shrani.**

Če zunanji pošiljatelji prejmejo napako, da nimate dovoljenja **(550 5.7.13),** zaženite ta ukaz v lupini [Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da si ogledate dovoljenja za anonimne uporabnike v javni mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` primer.

Če želite zunanjim uporabnikom omogočiti pošiljanje e-pošte v to javno mapo, dodajte dostop CreateItems uporabniku anonimno. Na `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` primer.
