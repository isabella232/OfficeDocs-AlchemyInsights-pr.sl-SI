---
title: Spreminjanje Microsoft Edge z uporabo spremenljivk podatkovnega imenika namesto hardcoded poti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679152"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Spreminjanje Microsoft Edge z uporabo spremenljivk podatkovnega imenika namesto hardcoded poti

Če želite na primer v sistemu Windows shraniti podatke profila v okviru uporabnikove lokalne aplikacije in ne na privzeto mesto, nastavite pravilnik **UserDataDir** na **$ {local_app_data} \Edge\Profile**. 

Če želite izvedeti več, glejte [Ustvarjanje spremenljivk za uporabniške podatke imenika Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).