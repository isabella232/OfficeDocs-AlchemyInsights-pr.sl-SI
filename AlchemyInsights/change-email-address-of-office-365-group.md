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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283261"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="85a03-102">Spreminjanje e-poštnega naslova skupine Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="85a03-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="85a03-103">E-poštni naslov skupine Microsoft 365 lahko spremenite s skrbniškim središčem.</span><span class="sxs-lookup"><span data-stu-id="85a03-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="85a03-104">Samo izberite skupino in izberite @edit e-poštni naslov.</span><span class="sxs-lookup"><span data-stu-id="85a03-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="85a03-105">Če želite spremeniti primarni naslov SMTP skupine Microsoft 365, lahko uporabite tudi naslednje ukaze EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="85a03-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="85a03-106">Set-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="85a03-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="85a03-107">Primer:</span><span class="sxs-lookup"><span data-stu-id="85a03-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
