---
title: Odpravljanje težav z dostavo e-pošte v javne mape z omogočeno pošto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716368"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Odpravljanje težav z dostavo e-pošte v javne mape z omogočeno pošto

Če zunanji pošiljatelji ne morejo pošiljati sporočil v javne mape z omogočenimi poštnimi sporočili, pošiljatelji pa prejmejo napako: **ni bilo mogoče najti (550 5.4.1)**, preveriti, ali je domena e-pošte za javno mapo konfigurirana kot notranja domena releja namesto avtoritativne domene:

1. Odprite [skrbniško središče za Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Pojdite na e- **poštni tok** \> **sprejete domene**, izberite sprejeto domeno in nato kliknite **Uredi**.

3. Na strani z lastnostmi, ki se odpre, če je vrsta domene nastavljena na **avtoritativno**, spremenite vrednost v **notranji rele** in nato kliknite **Shrani**.

Če zunanji pošiljatelji prejmejo napako, ki je nimate **dovoljenja (550 5.7.13)**, zaženite ta ukaz v [PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , da si ogledate dovoljenja za anonimne uporabnike v javni mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Če želite zunanjim uporabnikom omogočiti pošiljanje e-pošte v to javno mapo, dodajte pravico do dostopa CreateItems uporabniku anonimno. Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
