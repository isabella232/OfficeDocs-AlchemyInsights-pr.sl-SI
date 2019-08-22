---
title: Popraviti vprašanja dostave e-pošte za poštne javne mape
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525150"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Popraviti vprašanja dostave e-pošte za poštne javne mape

Če zunanjih pošiljateljev ne more pošiljati sporočil pošto javnih map, in oddajnik napaki: **ni bilo mogoče najti (550 5.4.1)**, preverite e-poštni domeni za javne mape je konfiguriran kot notranjo domeno za posredovanje namesto na avtoritativno domeno:

1. Odprite [izmenjavo admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Pojdi na **tok pošte** \> **sprejeto domene**, izberite sprejeto domeno, in nato kliknite **Urejanje**.

3. V lastnosti strani odpre, če domene tipa **Authoritative**, spremenite vrednost za **notranje posredovanje** in kliknite **Shrani**.

Če zunanjih pošiljateljev prikaže napaka, **nimate dovoljenja (550 5.7.13)**, zaženite ta ukaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , da vidite, katera dovoljenja za anonimne uporabnike v javni mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Zunanjim uporabnikom pošiljati email v tej javni mapi, dodajte CreateItems dostop pravico do uporabnika Anonymous. Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
