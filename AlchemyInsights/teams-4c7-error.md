---
title: Napaka» Teams 4c7 «
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700219"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="6ff12-102">Napaka 4c7 v aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6ff12-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="6ff12-103">Do te napake pride, ker Microsoft Teams zahteva preverjanje pristnosti obrazcev.</span><span class="sxs-lookup"><span data-stu-id="6ff12-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="6ff12-104">Ko uvedete storitve Active Directory Federation Services (AD FS), preverjanje pristnosti obrazcev privzeto ni omogočeno za intranet.</span><span class="sxs-lookup"><span data-stu-id="6ff12-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="6ff12-105">Če neuspešno preverjanje pristnosti sistema Windows ni uspelo, ste pozvani k vpisu s preverjanjem pristnosti obrazcev.</span><span class="sxs-lookup"><span data-stu-id="6ff12-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="6ff12-106">Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev tako, da uporabite snap-in konzolo Microsoft Management Console (MMC) v računalniku, v katerem je lokalna kopija imenika Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6ff12-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="6ff12-107">Če želite to narediti, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="6ff12-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="6ff12-108">V podoknu za krmarjenje Prebrskajte do **pravilnikov o preverjanju pristnosti**.</span><span class="sxs-lookup"><span data-stu-id="6ff12-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="6ff12-109">V razdelku **dejanja** v podoknu s podrobnostmi izberite **Uredi globalno primarno preverjanje pristnosti**.</span><span class="sxs-lookup"><span data-stu-id="6ff12-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="6ff12-110">Na zavihku **intranet** izberite **preverjanje pristnosti obrazcev**.</span><span class="sxs-lookup"><span data-stu-id="6ff12-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="6ff12-111">Izberite **v redu** (ali **uporabi**).</span><span class="sxs-lookup"><span data-stu-id="6ff12-111">Select **OK** (or **Apply**).</span></span>