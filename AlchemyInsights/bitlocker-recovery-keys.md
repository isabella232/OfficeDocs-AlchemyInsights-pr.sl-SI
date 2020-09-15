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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="b68bd-102">Dostop do obnovitvenih ključev BitLockerja</span><span class="sxs-lookup"><span data-stu-id="b68bd-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="b68bd-103">Ko konfigurirate nastavitve pogona BitLocker in nastavite pravilnik o zaščiti končnih točk, lahko določite, ali naj bodo podatki o obnovitvi BitLockerja shranjeni v imeniku Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b68bd-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="b68bd-104">Če je ta nastavitev konfigurirana, morajo biti shranjeni podatki za obnovitev vidni v obliki zapisa za InTune kot del podatkov o zapisu naprave v rezilu naprav za InTune na dva načina:</span><span class="sxs-lookup"><span data-stu-id="b68bd-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="b68bd-105">Naprave – naprave Azure AD – >» Device «ali naprave – > vse naprave – >» Device «– > obnovitvene tipke</span><span class="sxs-lookup"><span data-stu-id="b68bd-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="b68bd-106">Če pa obstaja skrbniški dostop do same naprave, je mogoče, da je obnovitveni ključ (geslo) videti tako, da zaženete ta ukaz v povišanem ukaznem pozivu:</span><span class="sxs-lookup"><span data-stu-id="b68bd-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="b68bd-107">Če je bila naprava pred vpisom šifrirana, je bil ključ za obnovitev morda povezan z» Microsoftovim računom «(MSA), ki se uporablja za vpis v napravo med postopkom OOBE.</span><span class="sxs-lookup"><span data-stu-id="b68bd-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="b68bd-108">Če je bilo to res, se lahko z dostopom  https://onedrive.live.com/recoverykey in vpisom v MSA prikaže naprave, za katere so bile shranjene obnovitvene tipke.</span><span class="sxs-lookup"><span data-stu-id="b68bd-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="b68bd-109">Če je bila naprava šifrirana zaradi konfiguracije prek pravilnika skupine, so lahko informacije o obnovitvi shranjene v imeniku Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b68bd-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

