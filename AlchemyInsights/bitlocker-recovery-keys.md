---
title: Obnovitveni ključi za Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060080"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Dostop do obnovitvenih ključev za Bitlocker

Pri konfiguriranju nastavitev za Bitlocker Pravilnik za zaščito končne točke za Intune lahko določite, ali naj bodo informacije o obnovitvi Bitlocker shranjene v Azure Active Directory.

Če je ta nastavitev konfigurirana, morajo biti shranjeni podatki za obnovitev vidni skrbniku za Intune kot del podatkov zapisa naprave v reji naprav storitve Intune na dva načina:

Naprave – naprave Azure AD -> »Naprava« ALI Naprave -> Vse naprave -> »Naprava« –> Obnovitveni ključi

Če pa imate skrbniški dostop do same naprave, si lahko obnovitveni ključ (Geslo) ogledali tako, da v ukaznem pozivu na skrbniški ravni zaženete ta ukaz:

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
Če je bila naprava šifrirana pred vpisom v Intune, je bil obnovitveni ključ morda povezan z Microsoftovim računom (MSA), ki se uporablja za vpis v napravo med postopkom OOBE. V tem primeru mora dostop do datoteke MSA in vpis z njim pokazati naprave, za katere so bili  https://onedrive.live.com/recoverykey shranjeni obnovitveni ključi.
 
Če je bila naprava šifrirana zaradi konfiguracije s pravilnikom skupine, ki temelji na domeni, se informacije o obnovitvi lahko shranijo v imenik Active Directory na mestu uporabe.

Če ste konfigurirali pravilnik za zaščito končne točke tako, da shrani obnovitveni ključ v Azure Active Directory vendar ključ za določeno napravo ni bil prenesen, lahko sprožite prenos tako, da za to napravo zasukate obnovitveni ključ iz konzole MEM. Če želite več podrobnosti, glejte [Sukanje obnovitvenih ključev za BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

