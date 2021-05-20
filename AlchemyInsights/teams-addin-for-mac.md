---
title: Teams dodatek za Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582086"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="8b8eb-102">Teams dodatek za Mac</span><span class="sxs-lookup"><span data-stu-id="8b8eb-102">Teams add-in for Mac</span></span>

<span data-ttu-id="8b8eb-103">Če želite odpraviti težave z manjkajo Teams za uporabnike dodatka za Mac, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="8b8eb-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="8b8eb-104">**1. korak:** Če uporabljate hibridno Exchange na mestu uporabe (2016 CU3 ali novejšo različico), z orodjem Test-HMA.ps1 preverite, ali je hibridno sodobno preverjanje pristnosti pravilno konfigurirano.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="8b8eb-105">Če želite več informacij, glejte [Preverjanje veljavnosti nastavitve hibridnega sodobnega preverjanja pristnosti Outlook za iOS in Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="8b8eb-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="8b8eb-106">**Opomba** Uporabite obliko zapisa naslova UPN (na primer [username@contoso.com](mailto:username@contoso.com)), ne domena\uporabniško ime.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="8b8eb-107">To naredite tudi za uporabnike z Exchange Online nabiralniki.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="8b8eb-108">**2. korak:** Uporabnik naj se po 9. po **12.**  >   v Outlook za Mac ter poiščite in izberite račun.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="8b8eb-109">Preverite, ali je navedeno uporabniško ime v obliki zapisa UPN (na [primer username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="8b8eb-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="8b8eb-110">**3. korak:** Preverite, ali je uporabnik licenciran Microsoft Teams uporabnik.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="8b8eb-111">Uporabnik mora uporabljati naročnino na Office 365 za Mac, različico izdelka 16.24 ali novejšo.</span><span class="sxs-lookup"><span data-stu-id="8b8eb-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>