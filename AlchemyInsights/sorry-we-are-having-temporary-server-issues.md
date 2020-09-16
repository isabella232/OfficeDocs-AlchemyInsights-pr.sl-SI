---
title: Odpravljanje težav s programom Microsoft 365 žal imamo sporočilo o začasnih težavah s strežnikom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758261"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Odpravljanje težav s storitvijo Microsoft 365» žal imamo sporočilo o začasnih težavah s strežnikom «

Če prejmete to sporočilo, naredite to:

1. Preverite požarni zid, protivirusno programsko opremo in nastavitve strežnika proxy, da potrdite, da ne blokirajo internetnega dostopa do programov Microsoft 365. Prikaz [URL-jev in obsegov naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Pojdite na **začetek**  >  **Zaženi**in vnesite **Services. msc**. Zagotovite, da se izvajajo te storitve:
    - Samodejna nastavitev omrežnih naprav, povezanih z omrežjem
    - Storitev omrežnega seznama
    - Poznavanje omrežnega mesta
    - Dnevnik dogodkov sistema Windows

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če imate težave z zagonom storitve, zaženite ta ukaz tako, da odprete ukazni poziv s povišanimi dovoljenji:

**SFC/scannow**

Ko se ukaz konča, znova zaženite računalnik.

Če želite podrobnejše informacije, glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Ko aktivirate sporočilo o napaki, poskusite znova](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).