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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816388"
---
# <a name="create-a-group"></a>Ustvarjanje skupine

V tej temi je opisano ustvarjanje skupin.

**Dovoljenje za ustvarjanje skupine**

Prepričajte se, da imate dovoljenje za ustvarjanje nove skupine. Globalni skrbniki lahko onemogočijo ustvarjanje skupin na portalu Azure ali v podoknu za dostop. Morda boste potrebovali skrbnika, ki bo ustvaril novo skupino za vas ali vam dal ustrezna dovoljenja.

**Upravljanje dovoljenj za ustvarjanje skupine**

1. Globalni skrbniki lahko upravljajo dovoljenja za ustvarjanje skupin (iz varnostnih razlogov) ali skupine v storitvi Office 365, ki so ustvarjene na portalu Azure ali v podoknu za dostop tako, da izberejo »Uporabniki lahko ustvarijo varnostne skupine v portalih Azure« ali »Uporabniki lahko ustvarijo skupine v storitvi Office 365 na portalih Azure« v razdelku Vse skupine Splošno  >  **(Nastavitve)**.
2. Prav tako lahko omejite ustvarjanje skupin, da izberete skupino uporabnikov, če imate licenco za Azure Active Directory P1 Premium.

**Onemogočanje pozdravnega obvestila za nove člane skupine v storitvi Office 365**

Pozdravno obvestilo, poslano uporabnikom, ki so bili dodani v skupine v storitvi Office 365, lahko onemogočite tako, da v ogrodju Powershell **UnifiedGroupWelcomeMessageEnabled** nastavite »False«. Več o tej nastavitvi [izveste tukaj.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

