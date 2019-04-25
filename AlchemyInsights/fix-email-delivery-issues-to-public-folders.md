---
title: Popraviti vprašanja dostave e-pošte za poštne javne mape
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401458"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Popraviti vprašanja dostave e-pošte za poštne javne mape

Če zunanjih pošiljateljev ne more pošiljati sporočil pošto javnih map, in oddajnik napaki: **ni bilo mogoče najti (550 5.4.1)**, preverite e-poštni domeni za javne mape je konfiguriran kot notranjo domeno za posredovanje namesto na avtoritativno domeno:

1. Odprite [izmenjavo admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Pojdi na **tok pošte** \> **sprejeto domene**, izberite sprejeto domeno, in nato kliknite **Urejanje**.

3. V lastnosti strani odpre, če domene tipa **Authoritative**, spremenite vrednost za **notranje posredovanje** in kliknite **Shrani**.

Če zunanjih pošiljateljev prikaže napaka, **nimate dovoljenja (550 5.7.13)**, zaženite ta ukaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , da vidite, katera dovoljenja za anonimne uporabnike v javni mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Zunanjim uporabnikom pošiljati email v tej javni mapi, dodajte CreateItems dostop pravico do uporabnika Anonymous. Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
