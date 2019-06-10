---
title: Preklic ali zamenjava e-pošto
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 461969bee3b871fd2c4a8418406ea2b6de791191
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770824"
---
# <a name="recall-or-replace-an-email-message"></a>Preklic ali zamenjava e-pošto

- Lahko **samo Preklic sporočila, ki so poslana ljudem v organizaciji**. Če je bilo sporočilo poslano na Gmail naslov, na primer, lahko ne spomnim to.
- Lahko **samo Preklic sporočila, poslana iz Outlook 2016 za PC**. Če uporabnik pošlje sporočilo z uporabo Outlook za Mac ali Outlook v spletu, lahko spomnim.
- Če ste admin, lahko **odpoklic sporočila v imenu uporabnikov z uporabo PowerShell**. Sporočila iz centra za admin ne more spomniti. Če želite več informacij, se pomaknite navzdol do "Iskanje in brisanje e-poštnih sporočil v vaši organizaciji".

***Preklic ali zamenjava e-poštno sporočilo, ki ste jo poslali***
1. V podoknu z mapami na levi strani Outlookovega okna, izberite mapo Poslano.
2. Odprite sporočilo, ki ga želite spomniti. Morate klikniti dvakrat, da odprete sporočilo. Izbiri sporočila, tako da se prikaže v podoknu za branje ne omogočajo Preklic sporočila.
3. Na kartici sporočilo, izberite **dejanja** > **Opozoriti na to sporočilo**.
4. Izberite **izbrisati neprebrane kopije tega sporočila** ali **izbrisati neprebrane kopije in zamenjati z novim sporočilom**, nato pa izberite **OK**.
5. Če pošiljate sporočilo zamenjavo, sestaviti sporočilo, nato pa izberite **Pošlji**.
6. Uspeh ali neuspeh Preklic sporočila je odvisna od nastavitve prejemnikov v Outlooku. 

Če želite več informacij, vključno s kako preverite na odpoklic, [preklic](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)ali Zamenjaj e-poštno sporočilo, ki ste jo poslali.

***Iskanje in brisanje e-poštnih sporočil v vaši organizaciji*** Iskanje in brisanje e-poštnih sporočil v vaši organizaciji, je najlažje, če ste svetovni admin. Če niste svetovnih admin, vaš račun je treba dodati skupini eDiscovery upravitelja vlog ali skladnost iskanje upravljalne vloge. Èe ¾elite zbrisati sporoèila, boste morali pridružiti skupine vlog »Upravljanje organizacije «ali iskanje in Počisti upravljalne vloge. Dovoljenja za te vloge so dodeljeni v [varnostni & skladnosti center](https://protection.office.com/).

1. [Ustvari vsebino iskanje](https://docs.microsoft.com/office365/securitycompliance/content-search) najti sporočilo za brisanje.
2. [Povezavo z varnostno & Center skladnosti PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Če uporabljate MFA, glejte [Vzpostavljanje povezave za Office 365 varnost & skladnosti Center PowerShell z uporabo multi-overjanja](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 