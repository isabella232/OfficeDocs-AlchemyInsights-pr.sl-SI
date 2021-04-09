---
title: Odpravljanje 0x8004de40 v storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649764"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="37e08-102">Odpravljanje 0x8004de40 v storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="37e08-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="37e08-103">Če uporabljate Windows 7 in se prikaže ta napaka, posodobite, da omogočite [TLS 1.1 in TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kot privzete varne protokole v sistemu WinHTTP v sistemu Windows.</span><span class="sxs-lookup"><span data-stu-id="37e08-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="37e08-104">Če imate nameščen Windows 10 in se prikaže sporočilo o 0x8004de40 v storitvi OneDrive:</span><span class="sxs-lookup"><span data-stu-id="37e08-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="37e08-105">Ko imate vzpostavljeno povezavo z domeno Acitve Directory, znova zaženite računalnik, v katerem to vpliva.</span><span class="sxs-lookup"><span data-stu-id="37e08-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="37e08-106">Če težave ne odpravite s ponovnim zagonom, se odklopite in se znova pridružite napravi v imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37e08-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="37e08-107">**Opomba:** V omrežju podjetja morate biti med izvajanjem teh korakov.</span><span class="sxs-lookup"><span data-stu-id="37e08-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="37e08-108">Teh korakov ne izvedite, če niste povezani s infrastrukturo podjetja (na primer med potovanjem).</span><span class="sxs-lookup"><span data-stu-id="37e08-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="37e08-109">Odprite ukazni poziv na skrbniški ravni tako, da izberete **Začetek**, z desno tipko miške kliknite **Ukazni** poziv in nato izberite **Zaženi kot skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="37e08-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="37e08-110">Vnesite *dsregcmd /leave in* pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="37e08-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="37e08-111">Ko končate, vnesite *dsregcmd /join in* pritisnite **tipko Enter**.</span><span class="sxs-lookup"><span data-stu-id="37e08-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="37e08-112">Ko je ukazni poziv dokončan, ga zaprite.</span><span class="sxs-lookup"><span data-stu-id="37e08-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="37e08-113">Znova zaženite računalnik in se prijavite v OneDrive.</span><span class="sxs-lookup"><span data-stu-id="37e08-113">Reboot the computer, and log into OneDrive.</span></span>