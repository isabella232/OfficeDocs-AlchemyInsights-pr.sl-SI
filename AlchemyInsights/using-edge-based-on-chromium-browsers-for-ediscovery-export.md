---
title: Uporaba brskalnika Microsoft Edge, ki temelji na brskalnikih Chromium za izvoz E-odkrivanja
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834387"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Uporaba brskalnika Microsoft Edge, ki temelji na brskalnikih Chromium za izvoz E-odkrivanja

Zaradi nedavne spremembe brskalniki Microsoft Edge ne bodo več privzeto omogočili podpore za ClickOnce. Če želite še naprej uporabljati orodje za izvoz e-odkrivanja v storitvi Microsoft 365, morate bodisi uporabiti Microsoft Internet Explorer ali omogočiti podporo za ClickOnce v brskalniku Microsoft Edge. 

Če želite omogočiti podporo za ClickOnce v brskalniku Microsoft Edge na osnovi brskalnika Chromium: 
1. V brskalniku Microsoft Edge obiščite spletno edge://flags/#edge-click-once.
2. Za možnost Podpora za ClickOnce  spremenite vrednost iz Privzeto ali **Onemogočeno** **v Omogočeno.** 
3. Na dnu okna brskalnika izberite Znova **zaženi**. <br>
 Sprememba bo veljati po vnovičnem zagonu brskalnika Microsoft Edge. 

Če želite več informacij o tem in korakih za namestitev orodja za izvoz, glejte: [Izvoz rezultatov iskanja vsebine.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)