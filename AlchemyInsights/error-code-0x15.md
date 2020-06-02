---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejmete napako, medtem ko aktivirate Office 2013 na uvajanje storitev oddaljenega namizja (RDS), razmislite o omogočanju ADAL z urejanjem registra.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506862"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Zmota prebiti activation urad 2013 naprej zakoten pult usluga

Če prejmete napako, medtem ko aktivirate Office 2013 na uvajanje storitev oddaljenega namizja (RDS), razmislite o omogočanju ADAL z urejanjem registra.
  
|**Registrski ključ**|**Vrsta**|**Vrednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Če želite več informacij, glejte [Omogočanje modernega preverjanja pristnosti za Office 2013 v napravah s sistemom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je privzeto omogočen v Microsoft 365 apps za podjetja in Office 2016. Storitve oddaljenega namizja (RDS) so bile prej imenovane terminalske storitve.
  