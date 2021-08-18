---
title: OneDrive napake pri prijavi AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112928"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive napake pri prijavi AADSTS50011

Če se pri vpisu v aplikacijo OneDrive prikaže napaka »AADSTS50011: URL odgovora, določen v zahtevi, se ne ujema z odgovorom«, preverite to:

Vaša OneDrive različica mora biti enaka ali večja od različice 20.052.XXXX.XXXX. Če želite preveriti različico, kliknite modro ikono OneDrive v območju za obvestila, izberite Pomoč **in & Nastavitve > Nastavitve > o.**

Vaše omrežje lahko blokira promet **v** g.live.com **in oneclient.sfx.ms.** Če je ta promet blokiran, se OneDrive mogoče posodobiti. Obrnite se na skrbnika omrežja in se prepričajte, da imate dostop do teh URL-jev. [Te končne točke morajo](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) doseči stranke, ki uporabljajo Microsoft 365 pakete.

Če morate ročno namestiti najnovejšo različico programa OneDrive, obiščite spletno mesto [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
