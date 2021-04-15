---
title: Napaka »Teams 4c7«
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786685"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="4f9f1-102">Napaka 4c7 v aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4f9f1-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="4f9f1-103">Do te napake pride, ker Microsoft Teams zahteva preverjanje pristnosti obrazcev.</span><span class="sxs-lookup"><span data-stu-id="4f9f1-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="4f9f1-104">Ko uvedete storitve AD FS (Active Directory Federation Services), preverjanje pristnosti obrazcev ni privzeto omogočeno za intranet.</span><span class="sxs-lookup"><span data-stu-id="4f9f1-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="4f9f1-105">Če integrirano preverjanje pristnosti sistema Windows ne uspe, ste pozvani k vpisu s preverjanjem pristnosti obrazcev.</span><span class="sxs-lookup"><span data-stu-id="4f9f1-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="4f9f1-106">Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev s snap-inom AD FS Microsoft Management Console (MMC) v računalniku, ki ima lokalno kopijo imenika Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f9f1-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="4f9f1-107">To naredite tako:</span><span class="sxs-lookup"><span data-stu-id="4f9f1-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="4f9f1-108">V podoknu za krmarjenje poiščite Pravilniki **za preverjanje pristnosti.**</span><span class="sxs-lookup"><span data-stu-id="4f9f1-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="4f9f1-109">V **razdelku Dejanja** v podoknu s podrobnostmi izberite Urejanje **globalnega primarnega preverjanja pristnosti.**</span><span class="sxs-lookup"><span data-stu-id="4f9f1-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="4f9f1-110">Na zavihku **Intranet** izberite Preverjanje **pristnosti obrazcev.**</span><span class="sxs-lookup"><span data-stu-id="4f9f1-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="4f9f1-111">Izberite **V redu** (ali **Uporabi).**</span><span class="sxs-lookup"><span data-stu-id="4f9f1-111">Select **OK** (or **Apply**).</span></span>