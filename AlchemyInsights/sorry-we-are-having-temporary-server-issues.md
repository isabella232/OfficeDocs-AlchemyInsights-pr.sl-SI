---
title: Pritrjevanje aplikacij za Microsoft 365 Žal mi je, da imamo začasno sporočilo o težavah strežnika
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582719"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Pritrjevanje Microsoft 365 apps "Oprostite, imamo začasna vprašanja strežnika" sporočilo

Če prejmete to sporočilo, poskusite naslednje:

1. Preverite požarni zid, protivirusno programsko opremo in nastavitve proxy, da potrdite, da ne blokira internetnega dostopa do Microsoftovih aplikacij za 365. Glejte [URL-je in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Iti k **začetek**  >  **prost dostop**, ter torej stavek **Services. msc**. Zagotovite, da se izvajajo naslednje storitve:
    - Samodejna nastavitev omrežne priključene naprave
    - Storitev omrežnega seznama
    - Omrežna lokacija zavedanje
    - Dnevnik dogodkov sistema Windows

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če vi življati a naloga odhod usluga, prost dostop sledeč zapoved z predrtina a zapoved uren s visok dovoljenje:

**SFC/scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Za podrobnejše informacije glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Poskusite znova pozneje "Napaka pri aktiviranju](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).