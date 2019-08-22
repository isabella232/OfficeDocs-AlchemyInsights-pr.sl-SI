---
title: Pretvarjanje nabiralnik uporabnika v nabiralnik v skupni rabi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496451"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Spremeniti uporabnik poštni nabiralnik v nabiralnik v skupni rabi

Nabiralnik uporabnika lahko pretvorite samo v nabiralnik v skupni rabi če uporabnik ima licenco za izmenjavo. Ko se pretvori v nabiralnik, bo še naprej kažejo na seznamu aktivnih uporabnikov, ker ta seznam vključuje nabiralniki v skupni rabi. Pa pretvori nabiralnika bo tudi prikazal na seznamu nabiralnik v skupni rabi. 
  
Če poskušate pretvoriti nabiralnik v Admin konzoli Exchange in pretvorba ne, vaš brskalnik predpomnilnik in piškotke in poskusite znova. Če to še vedno ne deluje, poskusite Pretvarjanje nabiralnik v programu Exchange Management Shell z tekmovanje v teku sledeč zapoved:
  
```
Set-Mailbox -Type Shared
```

Več nabiralnik pretvorba informacij je na voljo v [spremeniti uporabniškega nabiralnika za nabiralnik v skupni rabi](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
