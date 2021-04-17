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
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820302"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="2d5aa-102">Dostop do obnovitvenih ključev za Bitlocker</span><span class="sxs-lookup"><span data-stu-id="2d5aa-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="2d5aa-103">Pri konfiguriranju nastavitev za Bitlocker Pravilnik za zaščito končne točke za Intune lahko določite, ali naj bodo podatki za obnovitev Bitlocker shranjeni v imeniku Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="2d5aa-104">Če je ta nastavitev konfigurirana, morajo biti shranjeni podatki za obnovitev vidni skrbniku za Intune kot del podatkov zapisa naprave v reji naprav storitve Intune na dva načina:</span><span class="sxs-lookup"><span data-stu-id="2d5aa-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="2d5aa-105">Naprave – naprave Azure AD -> »Naprava« ALI Naprave -> Vse naprave -> »Naprava« –> Obnovitveni ključi</span><span class="sxs-lookup"><span data-stu-id="2d5aa-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="2d5aa-106">Če pa imate skrbniški dostop do same naprave, si lahko obnovitveni ključ (Geslo) ogledali tako, da v ukaznem pozivu na skrbniški ravni zaženete ta ukaz:</span><span class="sxs-lookup"><span data-stu-id="2d5aa-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="2d5aa-107">Če je bila naprava šifrirana pred vpisom v Intune, je bil obnovitveni ključ morda povezan z Microsoftovim računom (MSA), ki se uporablja za vpis v napravo med postopkom OOBE.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="2d5aa-108">V tem primeru mora dostop do datoteke MSA in vpis z njim pokazati naprave, za katere so bili  https://onedrive.live.com/recoverykey shranjeni obnovitveni ključi.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="2d5aa-109">Če je bila naprava šifrirana zaradi konfiguracije s pravilnikom skupine, ki temelji na domeni, se informacije o obnovitvi lahko shranijo v imenik Active Directory na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="2d5aa-110">Če ste konfigurirali pravilnik za zaščito končne točke tako, da shrani obnovitveni ključ v imeniku Azure Active Directory, vendar ključ za določeno napravo ni bil prenesen, lahko sprožite prenos tako, da za to napravo zasukate obnovitveni ključ iz konzole MEM.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="2d5aa-111">Če želite več podrobnosti, glejte [Sukanje obnovitvenih ključev za BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="2d5aa-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

