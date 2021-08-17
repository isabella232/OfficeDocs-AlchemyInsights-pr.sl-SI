---
title: Orodje za diagnostiko storitve za Windows navidezno namizje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052402"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Orodje za diagnostiko storitve za Windows navidezno namizje

Windows Navidezno namizje (WVD) ponuja diagnostično orodje, ki skrbnikom omogoča, da prepoznajo napake prek enega vmesnika. To orodje beleži diagnostične podatke vsakič, ko nekdo, ki ima dodeljeno vlogo WVD, uporabi WVD. V vsakem dnevniku so informacije o vlogi WVD, ki je vključena v dejavnost, sporočila o napakah, ki se prikažejo med sejo, in informacije o najemniku in uporabniku. Analitiko dnevnika Azure lahko konfigurirate tako, da zajame dnevnik dejavnosti, ustvarjen z diagnostičnim orodjem. To lahko:

1. Ustvarite delovni prostor Analitike dnevnika s [portalom Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ali [storitvijo Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Povezovalnik Windows računalnike v azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Pridobite ID delovnega prostora in primarni ključ delovnega prostora. Čarovnik za nastavitev potrebuje te informacije za pravilno konfiguracijo posrednika in za zagotavljanje, da lahko komunicira z nadzornikom Azure Monitor.
1. [Potisnete diagnostične podatke v delovni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Diagnostične podatke lahko potisnete iz najemnika WVD v analitiko dnevnikov za delovni prostor.
1. [Identificirajte in diagnosticiraj](https://go.microsoft.com/fwlink/?linkid=2128338) težave, ki so notranje ali zunanje glede na WVD.

Če želite izvedeti več o konfiguraciji orodja za diagnostiko storitve za WVD, glejte Uporaba analitike dnevnikov [za diagnostično funkcijo.](https://go.microsoft.com/fwlink/?linkid=2128084)
