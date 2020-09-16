---
title: Težava z aktiviranjem – trenutno se ne moremo povezati
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725999"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje programa Microsoft 365 apps» trenutno se ne moremo povezati s sporočilom «

Če prejmete to sporočilo, naredite to:

1. Preverite požarni zid, protivirusno programsko opremo in nastavitve strežnika proxy, da potrdite, da ne blokirajo internetnega dostopa do programov Microsoft 365. Oglejte si [Microsoftove URL-je in obsege naslovov IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Pojdite na **začetek**  >  **Zaženi**in vnesite **Services. msc**. Zagotovite, da se izvajajo te storitve:
    - Samodejna nastavitev omrežnih naprav, povezanih z omrežjem
    - Storitev omrežnega seznama
    - Poznavanje omrežnega mesta
    - Dnevnik dogodkov sistema Windows

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če imate težave z zagonom storitve, zaženite ta ukaz tako, da odprete ukazni poziv s povišanimi dovoljenji:

**SFC/scannow**

Ko se ukaz konča, znova zaženite računalnik.

Če želite podrobnejše informacije, glejte [» žal ne moremo vzpostaviti povezave z vašim računom. Ko aktivirate Office v storitvi Microsoft 365, poskusite znova» napaka «](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).