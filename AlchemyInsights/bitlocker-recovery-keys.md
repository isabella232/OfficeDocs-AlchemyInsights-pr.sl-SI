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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="7c889-102">Dostop do obnovitvene tipke BitLocker</span><span class="sxs-lookup"><span data-stu-id="7c889-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="7c889-103">Ko konfigurirate nastavitve za BitLocker InTune pravilnik o zaščiti končne točke, je mogoče določiti, ali naj se informacije o obnovitvi BitLocker shranijo v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c889-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="7c889-104">Če je ta nastavitev konfigurirana, morajo biti shranjeni podatki o obnovitvi vidni v InTune admin kot del podatkov o zapisu naprave v rezilo InTune naprave na dva načina:</span><span class="sxs-lookup"><span data-stu-id="7c889-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="7c889-105">Naprave-naprave Azure AD-> "naprava" ali naprave-> vse naprave-> "Device"-> obnovitvene tipke</span><span class="sxs-lookup"><span data-stu-id="7c889-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="7c889-106">Izmeničen, če je upraven postranski v načrt samo, regres zakleniti (parola) moči obstati seen z tekmovanje v teku sledeč zapoved s visok zapoved uren:</span><span class="sxs-lookup"><span data-stu-id="7c889-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="7c889-107">Če je bila naprava šifrirana pred vpisom v InTune, je obnovitveni ključ morda povezan z» Microsoftovim računom «(MSA), ki se uporablja za vpis v napravo med procesom OOBE.</span><span class="sxs-lookup"><span data-stu-id="7c889-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="7c889-108">Če bi bilo tako, dostop https://onedrive.live.com/recoverykey in vpis s tem MSA mora pokazati naprave, za katere so bili shranjeni ključi za obnovitev.</span><span class="sxs-lookup"><span data-stu-id="7c889-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="7c889-109">Če je bila naprava šifrirana zaradi konfiguracije prek pravilnika skupine, ki temelji na domeni, so informacije o obnovitvi morda shranjene v krajevnih imeniku Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c889-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

