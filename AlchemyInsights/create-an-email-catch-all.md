---
title: Ustvarjanje e-poštnega sporočila »Zasuti vse«
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
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080762"
---
# <a name="create-an-email-catch-all"></a>Ustvarjanje e-poštnega sporočila »Zasuti vse«

Uporaba catch all is strongly discouraged. Pošiljatelju raje pošljite sporočilo o tem, da sporočila ni bilo mogoče dostaviti kot obravnavano, zato da lahko ukrepajo. Nadzorujete lahko tudi nabiralnik, ki ste ga spremljali, in tako omejite, da v preteklosti velja le za veljavne e-poštne naslove. 

Vsaka zaseda vse nabiralnike prejme veliko neželene pošte in bo sčasoma lahko zapolnila, če ne bo skrbno nadzorovana. (Omejitve prejemanja.) 

Če želite nadaljevati, upoštevajte ta navodila:

1. Ustvarite dinamično skupino prejemnikov, & »All Recipient Types« (Vse vrste prejemnikov).

2. Ustvarite namenski nabiralnik, da zasukate e-poštna sporočila, na primer catchall@domain.com.

3. Za določeno domeno nastavite DomainType na »InternalRelay«. Če pozneje odstranite catch all (zajemi), ne glede na to, ali ste domeno nastavili nazaj na Avtoritativno.

4. Prenosno pravilo za poštni tok ustvarite tako:

    - Če je pošiljatelj »Zunaj organizacije«
    - Preusmeri sporočilo v Catchall@domain.com
    - Razen če je prejemnik član skupine allusers@domain.com (skupina prejemnikov vsebuje vse člane)
    - Preverite, ali so novi nabiralniki dodani v dinamično skupino prejemnikov
