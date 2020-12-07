---
title: Podpora Microsoft Edge za aplikacijo Microsoft Defender Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584010"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Podpora Microsoft Edge za aplikacijo Microsoft Defender Guard

Program Guard, zasnovan za Windows 10 in Microsoft Edge, uporablja način za izolacijo strojne opreme, ki uporabniku omogoča krmarjenje do nezaupanja vrednega mesta znotraj izoliranega vsebnika Hyper-V – omogočeno, ločen od gostiteljskega operacijskega sistema.

Skrbnik podjetja definira seznam zaupanja vrednih spletnih mest, virov v oblaku in notranjih omrežij. Ko uporabnik obišče mesto, ki ni na seznamu, bo Microsoft Edge odprl mesto v vsebniku. To pomeni, da bo v primeru, če se mesto izkaže kot zlonamerno, gostiteljski računalnik ostal zaščiten in napadalec ne bo mogel priti do podatkov podjetja.

Namestitev pripon v vsebniku je podprta z različico Microsoft Edge 81, ki jo je mogoče nadzorovati prek pravilnika. Naslov updateURL, ki se uporablja v pravilniku ExtensionInstallForcelist, je treba dodati kot nevtralni vir v pravilniku o izolaciji omrežja, ki ga uporablja skrbnik aplikacije.

Če želite več informacij, si oglejte [Microsoftova podpora za Microsoft Defender za aplikacijo Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
