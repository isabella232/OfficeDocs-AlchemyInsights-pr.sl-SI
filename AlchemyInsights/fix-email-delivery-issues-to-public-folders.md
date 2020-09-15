---
title: Odpravljanje težav z dostavo e-pošte v javne mape z omogočeno pošto
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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677944"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Odpravljanje težav z dostavo e-pošte v javne mape z omogočeno pošto

Če zunanji pošiljatelji ne morejo pošiljati sporočil v javne mape z omogočeno pošto in pošiljatelji prejmejo sporočilo o napaki: **ni bilo mogoče najti (550 5.4.1)**, preverite, ali je e-poštna domena za javno mapo konfigurirana kot notranja domena za posredovanje namesto avtoritativne domene:

1. Odprite [skrbniško središče za Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Pojdite na» **tok pošte** \> « **sprejete domene**, izberite sprejeto domeno in nato kliknite **Uredi**.

3. Na strani z lastnostmi, ki se odpre, če je vrsta domene nastavljena na **avtoritativno**, spremenite vrednost v **interno rele** in nato kliknite **Shrani**.

Če zunanji pošiljatelji prejmejo sporočilo o napaki, da nimate **dovoljenja (550 5.7.13)**, zaženite ta ukaz v [storitvi Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , da si ogledate dovoljenja za anonimne uporabnike v javni mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primer `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Če želite zunanjim uporabnikom omogočiti pošiljanje e-pošte v to javno mapo, dodajte CreateItems dostop do uporabnika Anonymous. Na primer `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
