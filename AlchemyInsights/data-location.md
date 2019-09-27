---
title: Lokacija podatkov
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207277"
---
# <a name="data-location"></a>Lokacija podatkov

Lokacijo vašega najemnika Office 365 si lahko ogledate v skrbniškem središču ali pa s povezavo na Exchange Online prek lupine PowerShell.


**Skrbniško središče:**
1. Prijavite se v [skrbniško središče](https://admin.microsoft.com/Adminportal/Home).
2. Izberite **Nastavitve** > **organizacije profil**.
3. Pod **lokacijo podatkov**izberite **Ogled podrobnosti**.


**Powershell:**
1. Z lupino Windows PowerShell vzpostavite povezavo s storitvijo Exchange Online.
2. Izvršiti [zaslužiti-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet razpoložiti a zapisati v seznam od vaš najemnik ' premožen. 
3. Poglejte lastnost OrganizationId.

Ko imate podatkovno lokacijo za EXO in SPO, lahko določite lokacijo podatkov za druge storitve, ki jih lahko uporabljate od koder se [nahajajo vaši podatki](https://products.office.com/where-is-your-data-located).