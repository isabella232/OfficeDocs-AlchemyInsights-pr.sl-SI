---
title: Orodje za diagnostiko storitve za navidezno namizje sistema Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596047"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Orodje za diagnostiko storitve za navidezno namizje sistema Windows

Navidezno namizje sistema Windows (WVD) ponuja diagnostično orodje, ki skrbnikom omogoča, da prepoznajo napake prek enega vmesnika. To orodje beleži diagnostične podatke vsakič, ko nekdo, ki ima dodeljeno vlogo WVD, uporabi WVD. V vsakem dnevniku so informacije o vlogi WVD, ki je vključena v dejavnost, sporočila o napakah, ki se prikažejo med sejo, in informacije o najemniku in uporabniku. Analitiko Azure Log Analytics lahko konfigurirate tako, da zajamete dnevnik dejavnosti, ustvarjen z diagnostičnim orodjem, tako da sledite tem korakom:

1. Ustvarite delovni prostor Analitike dnevnika s [portalom Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ali [storitvijo Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Povežite računalnike s sistemom Windows z orodjem Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Pridobite ID delovnega prostora in primarni ključ delovnega prostora. Čarovnik za nastavitev potrebuje te informacije za pravilno konfiguracijo posrednika in za zagotavljanje, da lahko komunicira z nadzornikom Azure Monitor.

1. [Potisnete diagnostične podatke v delovni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Diagnostične podatke lahko potisnete iz najemnika WVD v analitiko dnevnikov za delovni prostor.

1. [Identificirajte](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) in diagnosticiraj težave, ki so notranje ali zunanje glede na WVD.

Če želite izvedeti več o konfiguraciji orodja za diagnostiko storitve za WVD, glejte Uporaba analitike dnevnikov za diagnostično funkcijo.