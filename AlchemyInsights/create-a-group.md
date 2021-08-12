---
title: Ustvarjanje skupine
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
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929321"
---
# <a name="create-a-group"></a>Ustvarjanje skupine

V tej temi je opisano ustvarjanje skupin.

**Dovoljenje za ustvarjanje skupine**

Prepričajte se, da imate dovoljenje za ustvarjanje nove skupine. Globalni skrbniki lahko onemogočijo ustvarjanje skupin na portalu Azure ali v podoknu za dostop. Morda boste potrebovali skrbnika, ki bo ustvaril novo skupino za vas ali vam dal ustrezna dovoljenja.

**Upravljanje dovoljenj za ustvarjanje skupine**

1. Globalni skrbniki lahko upravljajo dovoljenja za ustvarjanje skupin (zaradi varnostnih razlogov) ali skupin Office 365, ustvarjenih na portalu Azure ali v accessski plošči, tako da v razdelku Vse skupine Splošno  >  **(Nastavitve)** izberete možnost »Uporabniki lahko ustvarijo varnostne skupine v portalih Azure« ali »Uporabniki lahko ustvarijo skupine Office 365 v portalih Azure«.
2. Prav tako lahko omejite ustvarjanje skupin tako, da izberete skupino uporabnikov, če imate Azure Active Directory P1 Premium licenco.

**Onemogočanje pozdravnega obvestila za nove Office 365 skupine**

Pozdravno obvestilo, poslano uporabnikom, ki so bili dodani v Office 365 lahko onemogočite tako, da v ogrodju Powershell **UnifiedGroupWelcomeMessageEnabled** nastavite »False«. Več o tej nastavitvi [izveste tukaj.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

