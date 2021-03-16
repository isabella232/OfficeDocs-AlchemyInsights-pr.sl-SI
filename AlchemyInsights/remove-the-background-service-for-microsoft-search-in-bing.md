---
title: Odstranjevanje storitve za ozadje za Microsoft Search v storitvi Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816338"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Odstranjevanje storitve za ozadje za Microsoft Search v storitvi Bing

Če želite odstraniti storitev za ozadje za Microsoft Search v storitvi Bing, lahko poskusite s temi sredstvi:

1. Če želite obnoviti prvotne nastavitve mehanizma za iskanje, naredite nekaj od tega:

    v. Preklapljanje med **uporabo storitve Bing kot privzetega [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) mehanizma za iskanje izklopite**.

    b. [Pojdite v skrbniško središče za Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) in počistite nastavitev, ki vpliva na vse uporabnike v vaši organizaciji.

2. Če želite odstraniti storitev za ozadje iz posamezne naprave, naredite ta opravila:

    v. Izberite **Nadzorna plošča > programi > programi in funkcijami**.

    b. Z desno tipko miške kliknite **Microsoft Search v storitvi Bing** pod seznamom nameščenih programov, nato pa kliknite **Odstrani**.

3. Če želite odstraniti storitev za ozadje iz več naprav v organizaciji, se prijavite kot skrbnik in zaženite ta ukaz v skriptu: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
