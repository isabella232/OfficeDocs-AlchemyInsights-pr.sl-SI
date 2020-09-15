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
description: Če prejmete sporočilo o napaki, medtem ko aktivirate Office 2013 za uvajanje oddaljenih namiznih storitev (RDS), razmislite o tem, kako omogočite knjižnice ADAL z urejanjem registra.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709203"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Napaka pri aktivaciji sistema Office 2013 v storitvah oddaljenega namizja

Če prejmete sporočilo o napaki, medtem ko aktivirate Office 2013 za uvajanje oddaljenih namiznih storitev (RDS), razmislite o tem, kako omogočite knjižnice ADAL z urejanjem registra.
  
|**Registrski ključ**|**Vnesite**|**Vrednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Če želite več informacij, glejte [Omogočanje sodobnega preverjanja pristnosti za Office 2013 v napravah s sistemom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  KNJIŽNICE ADAL je privzeto omogočen v programih Microsoft 365 za podjetja in Office 2016. Oddaljenega namiznih storitev (RDS) je bilo prej imenovanih terminalskih storitev.
  