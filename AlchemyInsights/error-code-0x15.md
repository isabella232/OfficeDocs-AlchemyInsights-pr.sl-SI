---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527066"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Napaka pri aktiviranje Office 2013 na storitev oddaljenega namizja.

Če prejemate napake med aktiviranjem urad 2013 na uvajanje oddaljenega namizja storitve (RDS), menijo, ki omogoča ADAL z urejanjem registra.
  
|**Registrski ključ**|**Vrsta**|**Vrednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Če želite več informacij, glejte [Omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  FRENKX je privzeto omogočena v Office 365 ProPlus in Office 2016. Oddaljenega namizja storitve (RDS) je bil prej imenovan terminalskih storitev.
  