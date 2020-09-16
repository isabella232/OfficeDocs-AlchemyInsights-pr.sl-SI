---
title: Dodatek» Teams «za Mac
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670344"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="01d5e-102">Dodatek» Teams «za Mac</span><span class="sxs-lookup"><span data-stu-id="01d5e-102">Teams add-in for Mac</span></span>

<span data-ttu-id="01d5e-103">Če želite odpraviti težave z manjkajočim dodatkom Teams za računalnike Mac, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="01d5e-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="01d5e-104">**1. korak:** Če imate hibridno Exchange na mestu uporabe (2016 CU3 ali novejšo), uporabite orodje Test-HMA.ps1, da preverite, ali je hibridno sodobno preverjanje pristnosti pravilno konfigurirano.</span><span class="sxs-lookup"><span data-stu-id="01d5e-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="01d5e-105">Če želite več informacij, si oglejte [preverjanje veljavnosti hibridnega sodobnega nastavitev preverjanja pristnosti za Outlook za iOS in Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="01d5e-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="01d5e-106">**Opomba** Uporabite obliko naslova UPN (na primer [username@contoso.com](mailto:username@contoso.com)), ne DOMAIN\username.</span><span class="sxs-lookup"><span data-stu-id="01d5e-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="01d5e-107">To naredite tudi za uporabnike s poštnimi nabiralniki Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="01d5e-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="01d5e-108">**2. korak:** Naj se uporabnik povrne na **Orodja**za  >  **račune**... v programu Outlook for Mac in poiščite in izberite račun.</span><span class="sxs-lookup"><span data-stu-id="01d5e-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="01d5e-109">Potrdite, da je navedeno uporabniško ime v obliki zapisa UPN (na primer [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="01d5e-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="01d5e-110">**3. korak:** Potrdite, da je uporabnik licenciran Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="01d5e-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="01d5e-111">Uporabnik mora uporabljati naročnino na Office 365 za Mac, različica izdelka 16,24 ali novejšo različico.</span><span class="sxs-lookup"><span data-stu-id="01d5e-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>