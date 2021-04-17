---
title: Sprememba e-poštnega naslova skupine v storitvi Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819060"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="4adfd-102">Sprememba e-poštnega naslova skupine v storitvi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4adfd-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="4adfd-103">E-poštni naslov skupine v storitvi Microsoft 365 lahko spremenite v skrbniškem središču.</span><span class="sxs-lookup"><span data-stu-id="4adfd-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="4adfd-104">Izberite skupino, nato pa izberite »@Uredi e-poštni naslov«.</span><span class="sxs-lookup"><span data-stu-id="4adfd-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="4adfd-105">Primarni naslov SMTP za skupino v storitvi Microsoft 365 lahko spremenite tudi s sledečim ukazom EXO Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4adfd-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="4adfd-106">Niz-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="4adfd-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="4adfd-107">Primer:</span><span class="sxs-lookup"><span data-stu-id="4adfd-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
