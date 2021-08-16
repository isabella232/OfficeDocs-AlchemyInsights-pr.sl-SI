---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če med aktiviranjem sistema Office 2013 v uvajanjih storitev oddaljenega namizja (RDS) prejemate sporočilo o napaki, razmislite o tem, da bi omogočili ADAL z urejanjem registra.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100778"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Napaka med aktiviranjem Office 2013 v storitvah oddaljenega namizja

Če med aktiviranjem sistema Office 2013 v uvajanjih storitev oddaljenega namizja (RDS) prejemate sporočilo o napaki, razmislite o tem, da bi omogočili ADAL z urejanjem registra.
  
|**Registrski ključ**|**Vrsta**|**Vrednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Če želite več informacij, [glejte Omogočanje sodobnega preverjanja pristnosti Office 2013 v Windows napravah.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL je privzeto omogočena v brskalnikih Programi Microsoft 365 za podjetja in Office 2016. Storitev oddaljenega namizja (RDS) se je v preteklosti imenovala terminalske storitve.
  