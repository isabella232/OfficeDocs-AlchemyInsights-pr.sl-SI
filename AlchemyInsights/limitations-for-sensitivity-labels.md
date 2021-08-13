---
title: Omejitve za oznake občutljivosti za Office datotek v SharePoint in OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813167"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Omejitve za oznake občutljivosti za Office datotek v SharePoint in OneDrive

Ko želite omogočiti oznake občutljivosti Office datotek v SharePoint in OneDrive, bodite pozorni na zahteve in omejitve, ki vključujejo:

- SharePoint in OneDrive ne moreta obdelati nekaterih datotek, ki so označene in šifrirane v namiznih programih sistema Office, če datoteke vsebujejo podatke PowerQuery, podatke, shranjene z dodatki po meri ali deli XML po meri.
- SharePoint in OneDrive ne uporabite samodejno oznak občutljivosti za obstoječe datoteke, ki ste jih že šifrirani z oznakami Azure Information Protection (AIP). Če želite za šifrirane datoteke uporabiti oznake občutljivosti: 
    - Prepričajte se, da so bile oznake AIP preseljene in objavljene v središču za Microsoft 365 za skladnost s predpisi.
    - Prenesite označene datoteke in jih nato naložite na prvotno mesto SharePoint ali OneDrive mesta.
- Za šifrirane dokumente tiskanje ni podprto.

Če želite dodatne podrobnosti o omejitvah, [glejte Omogočanje oznak občutljivosti za Office datotek v mapah SharePoint in OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
