---
title: Težava z aktiviranjem – trenutno ni mogoče vzpostaviti povezave
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998179"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje Microsoft 365 »Povezave trenutno ni mogoče vzpostaviti«

Če se prikaže to sporočilo, poskusite to:

1. Preverite nastavitve požarnega zidu, protivirusne programske opreme in strežnika proxy ter se prepričajte, da ne blokirajo dostopa do Microsoft 365 programov. Glejte [Microsoftovi URL-ji in obsegi naslovov IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Odprite začetni **meni**  >  **Zaženi** in vnesite **services.msc**. Prepričajte se, da so vse te storitve zagnane:
    - Samodejna nastavitev naprav, povezanih z omrežjem
    - Omrežna storitev seznama
    - Ozaveščenost o omrežnem mestu
    - Windows Dnevnik dogodkov

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če imate težave pri zagonu storitve, zaženite ta ukaz tako, da odprete ukazni poziv z povečanimi dovoljenji:

**sfc /scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Če želite podrobne informacije, glejte [»Povezave z vašim računom žal ni mogoče vzpostaviti. Poskusite znova pozneje«, ko aktivirate sistem Office v Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)