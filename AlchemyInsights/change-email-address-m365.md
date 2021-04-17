---
title: Spreminjanje e-poštnega naslova skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819096"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="a18e7-102">Spreminjanje e-poštnega naslova skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a18e7-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="a18e7-103">E-poštni naslov skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams lahko spremenite v [Skrbniškem središču za Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="a18e7-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="a18e7-104">Izberite skupino, nato pa izberite »@Uredi e-poštni naslov«.</span><span class="sxs-lookup"><span data-stu-id="a18e7-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="a18e7-105">Primarni naslov SMTP za skupino v okolju Microsoft 365 ali aplikacijo Teams lahko spremenite tudi s tem ukazom EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a18e7-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="a18e7-106">Primer:</span><span class="sxs-lookup"><span data-stu-id="a18e7-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
