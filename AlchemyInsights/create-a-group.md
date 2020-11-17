---
title: Ustvarjanje skupine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089176"
---
# <a name="create-a-group"></a>Ustvarjanje skupine

V tej temi je opisana ustvarjanje skupine.

**Dovoljenje za ustvarjanje skupine**

Zagotovite, da imate dovoljenje za ustvarjanje nove skupine. Globalni skrbniki lahko onemogočijo ustvarjanje skupine v portalu Azure ali v Accessovi plošči. Morda boste potrebovali skrbnika, če želite ustvariti novo skupino za vas ali pa vam dati ustrezna dovoljenja.

**Upravljanje dovoljenj za ustvarjanje skupin**

1. Globalni skrbniki lahko upravljajo dovoljenja za ustvarjanje skupin (zaradi varnostnih razlogov) ali skupin Office 365, ki so bile ustvarjene v portalu Azure ali Accessovi plošči, tako da izberete» uporabniki lahko ustvarijo varnostne skupine v storitvi Azure portali «ali» uporabniki lahko ustvarijo Office 365 skupine v storitvi Azure Portals «v razdelku» **vse skupine**«  >  **(nastavitve)**.
2. Lahko tudi omejite ustvarjanje skupine, če želite izbrati skupino uporabnikov, če imate licenco Azure Active Directory P1 Premium.

**Onemogočanje pozdravne priglasitve za nove člane skupine v sistemu Office 365**

Pozdravno obvestilo, poslano uporabnikom, ki so dodani v skupine sistema Office 365, lahko onemogočite tako, da nastavite **UnifiedGroupWelcomeMessageEnabled** na False v lupini PowerShell. Preberite več o tej nastavitvi [tukaj](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

