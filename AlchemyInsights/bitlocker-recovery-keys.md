---
title: Obnovitveni ključi za BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685902"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Dostop do obnovitvenih ključev BitLockerja

Ko konfigurirate nastavitve pogona BitLocker in nastavite pravilnik o zaščiti končnih točk, lahko določite, ali naj bodo podatki o obnovitvi BitLockerja shranjeni v imeniku Azure Active Directory.

Če je ta nastavitev konfigurirana, morajo biti shranjeni podatki za obnovitev vidni v obliki zapisa za InTune kot del podatkov o zapisu naprave v rezilu naprav za InTune na dva načina:

Naprave – naprave Azure AD – >» Device «ali naprave – > vse naprave – >» Device «– > obnovitvene tipke

Če pa obstaja skrbniški dostop do same naprave, je mogoče, da je obnovitveni ključ (geslo) videti tako, da zaženete ta ukaz v povišanem ukaznem pozivu:

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
Če je bila naprava pred vpisom šifrirana, je bil ključ za obnovitev morda povezan z» Microsoftovim računom «(MSA), ki se uporablja za vpis v napravo med postopkom OOBE. Če je bilo to res, se lahko z dostopom  https://onedrive.live.com/recoverykey in vpisom v MSA prikaže naprave, za katere so bile shranjene obnovitvene tipke.
 
Če je bila naprava šifrirana zaradi konfiguracije prek pravilnika skupine, so lahko informacije o obnovitvi shranjene v imeniku Active Directory.
 

