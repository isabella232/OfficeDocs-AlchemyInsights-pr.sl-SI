---
title: Odpravljanje težav s preverjanjem pristnosti SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826431"
---
# <a name="solving-smtp-authentication-issues"></a>Odpravljanje težav s preverjanjem pristnosti SMTP

Če se pri poskusu pošiljanja e-pošte strežnika SMTP napake 5.7.57 ali 5.7.3 in preverijo pristnost z odjemalcem ali aplikacijo, preverite nekaj stvari:

- Pošiljanje SMTP s preverjeno pristnostjo je morda onemogočeno v najemniku ali v nabiralniku, ki ga želite uporabiti (preverite obe nastavitva). Če želite več informacij, glejte [Omogočanje ali onemogočanje pošiljanja SMTP odjemalca s preverjeno pristnostjo.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Preverite, [ali so za vašega](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) najemnika omogočene privzete nastavitve za Varnost Azure; Če je omogočeno, preverjanje pristnosti SMTP z osnovnim preverjanjem pristnosti (znano tudi kot podedovano; s tem uporabniškim imenom in geslom) ne bo uspelo.
