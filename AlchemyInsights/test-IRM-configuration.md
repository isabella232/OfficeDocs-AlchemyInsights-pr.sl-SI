---
title: Preskus konfiguracije upravljanja pravic do informacij za nove zmogljivosti za OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812447"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Preskus konfiguracije upravljanja pravic do informacij za nove zmogljivosti za OME

Če želite preveriti, ali Microsoft 365 najemnik konfiguriran za uporabo novih zmogljivosti za OME, zaženite te ukaze »cmdlet« med Exchange Online [PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Preverite konfiguracijo upravljanja pravic do informacij najemnika tako, da zaženete `Get-IRMConfiguration` . Prepričajte se, da so te vrednosti nastavljene na **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Z domeno, naslovom pošiljatelja in prejemnikom zaženite `Test-IRMConfiguration` . Če preskus ni uspešno preu iten, raziščite konfiguracijo upravljanja pravic do informacij.

Če želite več informacij o tem, kako preverite konfiguracijo upravljanja pravic do informacij, [glejte Preverjanje nove konfiguracije za OME v Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)