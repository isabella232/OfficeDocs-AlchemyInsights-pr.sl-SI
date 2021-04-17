---
title: Popravljanje programov storitve Microsoft 365 Žal je na voljo sporočilo o začasnih težavah s strežnikom
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
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835287"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Če popravite programe storitve Microsoft 365, se prikaže sporočilo »Žal imamo začasne težave s strežnikom«

Če se prikaže to sporočilo, poskusite to:

1. Preverite nastavitve požarnega zidu, protivirusne programske opreme in strežnika proxy, da potrdite, da ne blokirajo dostopa do interneta do aplikacij storitve Microsoft 365. Glejte [URL-ji in obsegi naslovov IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Odprite začetni **meni**  >  **Zaženi** in vnesite **services.msc**. Prepričajte se, da so vse te storitve zagnane:
    - Samodejna nastavitev naprav, povezanih z omrežjem
    - Omrežna storitev seznama
    - Ozaveščenost o omrežnem mestu
    - Dnevnik dogodkov sistema Windows

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če imate težave pri zagonu storitve, zaženite ta ukaz tako, da odprete ukazni poziv z povečanimi dovoljenji:

**sfc /scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Če želite podrobne informacije, glejte [»Povezave z vašim računom žal ni mogoče vzpostaviti. Pri aktiviranju se prikaže napaka »Poskusite znova pozneje«.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)