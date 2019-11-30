---
title: Pritrjevanje Officeovih aplikacij Žal mi je, da imamo sporočilo o začasnih težavah s strežnikom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628006"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Popravljanje Officeovih aplikacij» Žal mi je, da imamo sporočilo o začasnih težavah v strežniku «

Če prejmete to sporočilo, poskusite naslednje:

1. Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Officeovih aplikacij. Glejte [URL-je sistema Office 365 in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Iti k **začetek** > **prost dostop**, ter torej stavek **Services. msc**. Zagotovite, da se izvajajo naslednje storitve:
    - Samodejna nastavitev omrežne priključene naprave
    - Storitev omrežnega seznama
    - Omrežna lokacija zavedanje
    - Dnevnik dogodkov sistema Windows

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:

**SFC/scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "napako, ko aktivirate Office iz Officea 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).