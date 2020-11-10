---
title: Napaka pri prijavi OneDrive AADSTS50011
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982546"
---
# <a name="onedrive-login-error-aadsts50011"></a>Napaka pri prijavi OneDrive AADSTS50011

Če prejmete sporočilo o napaki» AADSTS50011: URL odgovora, ki je naveden v zahtevi, se ne ujema z odgovorom «, ko se vpišete v program OneDrive, poiščite to:

Vaša različica OneDrive mora biti enaka ali večja od različice 20.052. XXXX. XXXX. Če želite preveriti različico, kliknite ikono modrega OneDrive v območju za obvestila, nato **pa izberite pomoč & nastavitve > nastavitve >**.

Omrežje lahko blokira promet v **g.Live.com** in **oneclient.SFX.MS**. Če je promet blokiran, se OneDrive ne more posodobiti. Delo s skrbnikom omrežja, da zagotovite dostop do teh URL-jev. [Te končne točke](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) bi morale biti dosegljive za stranke, ki uporabljajo programe Microsoft 365.

Če morate ročno pridobiti trenutno različico programa OneDrive, obiščite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
