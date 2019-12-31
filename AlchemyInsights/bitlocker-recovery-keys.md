---
title: Obnovitvene tipke za BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908830"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Dostop do obnovitvene tipke BitLocker

Ko konfigurirate nastavitve za BitLocker InTune pravilnik o zaščiti končne točke, je mogoče določiti, ali naj se informacije o obnovitvi BitLocker shranijo v storitvi Azure Active Directory.

Če je ta nastavitev konfigurirana, morajo biti shranjeni podatki o obnovitvi vidni v InTune admin kot del podatkov o zapisu naprave v rezilo InTune naprave na dva načina:

Naprave-naprave Azure AD-> "naprava" ali naprave-> vse naprave-> "Device"-> obnovitvene tipke

Izmeničen, če je upraven postranski v načrt samo, regres zakleniti (parola) moči obstati seen z tekmovanje v teku sledeč zapoved s visok zapoved uren:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Če je bila naprava šifrirana pred vpisom v InTune, je obnovitveni ključ morda povezan z» Microsoftovim računom «(MSA), ki se uporablja za vpis v napravo med procesom OOBE. Če bi bilo tako, dostop https://onedrive.live.com/recoverykey in vpis s tem MSA mora pokazati naprave, za katere so bili shranjeni ključi za obnovitev.
 
Če je bila naprava šifrirana zaradi konfiguracije prek pravilnika skupine, ki temelji na domeni, so informacije o obnovitvi morda shranjene v krajevnih imeniku Active Directory.
 

