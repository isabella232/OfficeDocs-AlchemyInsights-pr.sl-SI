---
title: Activation Issue-ne moremo povezati prav zdaj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716188"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje Officeovih aplikacij» trenutno ne moremo vzpostaviti sporočila «

Če prejmete to sporočilo, poskusite naslednje:

1. Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Officeovih aplikacij. Glejte [Microsoft URL-ji in obsegi naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Iti k **začetek** > **prost dostop**, ter torej stavek **Services. msc**. Zagotovite, da se izvajajo naslednje storitve:
    - Samodejna nastavitev omrežne priključene naprave
    - Storitev omrežnega seznama
    - Omrežna lokacija zavedanje
    - Dnevnik dogodkov sistema Windows

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:

**SFC/scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "napako, ko aktivirate Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).