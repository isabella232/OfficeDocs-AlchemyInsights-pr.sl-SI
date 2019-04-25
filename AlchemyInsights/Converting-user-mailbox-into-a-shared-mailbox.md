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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374339"
---
Nabiralnik uporabnika lahko pretvorite samo v nabiralnik v skupni rabi če uporabnik ima licenco za izmenjavo. Ko se pretvori v nabiralnik, bo še naprej kažejo na seznamu aktivnih uporabnikov, ker ta seznam vključuje nabiralniki v skupni rabi. Pa pretvori nabiralnika bo tudi prikazal na seznamu nabiralnik v skupni rabi. 
  
Če poskušate pretvoriti nabiralnik v Admin konzoli Exchange in pretvorba ne, vaš brskalnik predpomnilnik in piškotke in poskusite znova. Če to še vedno ne deluje, poskusite Pretvarjanje nabiralnik v programu Exchange Management Shell z tekmovanje v teku sledeč zapoved:
  
```
Set-Mailbox -Type Shared
```

Več nabiralnik pretvorba informacij je na voljo v [spremeniti uporabniškega nabiralnika za nabiralnik v skupni rabi](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
