---
title: Spreminjanje e-poštnega naslova skupine Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580673"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="f8a14-102">Spreminjanje e-poštnega naslova skupine Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f8a14-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="f8a14-103">E-poštni naslov skupine Microsoft 365 lahko spremenite s skrbniškim središčem.</span><span class="sxs-lookup"><span data-stu-id="f8a14-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="f8a14-104">Samo izberite skupino in izberite @edit e-poštni naslov.</span><span class="sxs-lookup"><span data-stu-id="f8a14-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="f8a14-105">Če želite spremeniti primarni naslov SMTP skupine Microsoft 365, lahko uporabite tudi naslednje ukaze EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f8a14-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="f8a14-106">Set-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="f8a14-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="f8a14-107">Primer:</span><span class="sxs-lookup"><span data-stu-id="f8a14-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
