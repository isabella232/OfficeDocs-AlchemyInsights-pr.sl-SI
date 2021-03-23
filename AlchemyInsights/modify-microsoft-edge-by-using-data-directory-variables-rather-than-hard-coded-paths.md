---
title: Spremenite Microsoft Edge s spremenljivkami podatkovnega imenika in ne z nekodiranimi potmi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036857"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Spremenite Microsoft Edge s spremenljivkami podatkovnega imenika in ne z nekodiranimi potmi

Če želite na primer v sistemu Windows shraniti podatke profila v okviru uporabnikove lokalne aplikacije in ne na privzeto mesto, nastavite pravilnik *UserDataDir* na **$ {local_app_data} \Edge\Profile**.

Če želite več informacij, glejte [Ustvarjanje spremenljivk za uporabniške podatke imenika Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).