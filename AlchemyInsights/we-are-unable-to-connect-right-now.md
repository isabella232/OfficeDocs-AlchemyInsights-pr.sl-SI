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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744611"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje Microsoft 365 »Povezave trenutno ni mogoče vzpostaviti«

Opomba: Če uporabljate starejšo različico programa Windows (npr. Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), uporabite preprost popravek, da za privzeto omogočite TLS 1.2. Če želite več informacij, glejte Posodobitev, da omogočite [TLS 1.1 in TLS 1.2 kot](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)privzete varne protokole v winhttp v brskalniku Windows.

Če se prikaže to sporočilo, poskusite to:

1. Preverite nastavitve požarnega zidu, protivirusne programske opreme in strežnika proxy, da potrdite, da ne blokirajo dostopa do Microsoft 365 programov. Glejte [Microsoftovi URL-ji in obsegi naslovov IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Odprite začetni **meni**  >  **Zaženi** in vnesite **services.msc**. Prepričajte se, da so vse te storitve zagnane:
    - Samodejna nastavitev v omrežnih napravah
    - Omrežna storitev seznama
    - Ozaveščenost o omrežnem mestu
    - Windows Dnevnik dogodkov

Če se ena od teh storitev ne izvaja, jo poskusite zagnati. Če imate težave pri zagonu storitve, zaženite ta ukaz tako, da odprete ukazni poziv z povečanimi dovoljenji:

**sfc /scannow**

Ko se ta ukaz dokonča, znova zaženite računalnik.

Če želite podrobne informacije, glejte [»Povezave z vašim računom žal ni mogoče vzpostaviti. Poskusite znova pozneje«, ko aktivirate sistem Office iz Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).