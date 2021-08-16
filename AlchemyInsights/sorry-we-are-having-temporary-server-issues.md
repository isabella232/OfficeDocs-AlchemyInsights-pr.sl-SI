---
title: Odpravljanje Microsoft 365 programov Žal imamo sporočilo o začasnih težavah s strežnikom
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021612"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Če popravite Microsoft 365 se prikaže sporočilo »Žal imamo začasne težave s strežnikom«

Če se prikaže to sporočilo, poskusite to:

1. Preverite nastavitve požarnega zidu, protivirusne programske opreme in strežnika proxy ter se prepričajte, da ne blokirajo dostopa do Microsoft 365 programov. Glejte [URL-ji in obsegi naslovov IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Odprite začetni **meni**  >  **Zaženi** in vnesite **services.msc**. Prepričajte se, da so vse te storitve zagnane:
    - Samodejna nastavitev naprav, povezanih z omrežjem
    - Omrežna storitev seznama
    - Ozaveščenost o omrežnem mestu
    - Windows Dnevnik dogodkov

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če imate težave pri zagonu storitve, zaženite ta ukaz tako, da odprete ukazni poziv z povečanimi dovoljenji:

**sfc /scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Če želite podrobne informacije, glejte [»Povezave z vašim računom žal ni mogoče vzpostaviti. Pri aktiviranju se prikaže napaka »Poskusite znova pozneje«.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)