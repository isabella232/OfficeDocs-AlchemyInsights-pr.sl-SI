---
title: Napaka 4c7 ekipe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796376"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="33eb2-102">4c7 napaka v Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="33eb2-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="33eb2-103">Do te napake pride, ker Microsoft Teams zahteva preverjanje pristnosti obrazcev.</span><span class="sxs-lookup"><span data-stu-id="33eb2-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="33eb2-104">Ko uvedete storitve Active Directory Federation Services (AD FS), preverjanje pristnosti obrazcev ni privzeto omogočeno za intranet.</span><span class="sxs-lookup"><span data-stu-id="33eb2-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="33eb2-105">Če okno enoten Authentication ne zadostovati, vi ste sufler v znamenje v using obrazec Authentication.</span><span class="sxs-lookup"><span data-stu-id="33eb2-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="33eb2-106">Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev tako, da v računalniku, v katerem je lokalna kopija imenika Active Directory, uporabite snap-in MMC konzole AD FS.</span><span class="sxs-lookup"><span data-stu-id="33eb2-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="33eb2-107">Če želite to narediti, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="33eb2-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="33eb2-108">V podoknu za krmarjenje Prebrskajte do **pravilnikov o preverjanju pristnosti**.</span><span class="sxs-lookup"><span data-stu-id="33eb2-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="33eb2-109">V razdelku **dejanja** v podoknu s podrobnostmi izberite **Uredi globalno primarno preverjanje pristnosti**.</span><span class="sxs-lookup"><span data-stu-id="33eb2-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="33eb2-110">Na zavihku **intranet** izberite **preverjanje pristnosti obrazcev**.</span><span class="sxs-lookup"><span data-stu-id="33eb2-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="33eb2-111">Izberite **v redu** (ali **uporabite**).</span><span class="sxs-lookup"><span data-stu-id="33eb2-111">Select **OK** (or **Apply**).</span></span>