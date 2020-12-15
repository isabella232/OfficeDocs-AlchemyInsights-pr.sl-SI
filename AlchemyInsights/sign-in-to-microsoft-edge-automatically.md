---
title: Samodejno vpis v Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678816"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="a4388-102">Samodejno vpis v Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a4388-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="a4388-103">Microsoft Edge uporablja privzeti račun OS za samodejno vpis uporabnika glede na to, kako je uporabnikova naprava konfigurirana.</span><span class="sxs-lookup"><span data-stu-id="a4388-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="a4388-104">Scenariji za vsako vrsto konfiguracije naprave in njegovega odvisnega postopka za vpis uporabnika so opisani spodaj:</span><span class="sxs-lookup"><span data-stu-id="a4388-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="a4388-105">**Naprava je hibridna/zvočna – J**: Ta možnost je na voljo v sistemu Windows 10, sistemu Windows in ustreznih različicah strežnika.</span><span class="sxs-lookup"><span data-stu-id="a4388-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="a4388-106">Uporabniki so samodejno vpisani s svojimi računi v storitvi Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="a4388-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="a4388-107">**Naprava je povezana z domeno**: Ta možnost je na voljo v sistemu Windows 10, sistemu Windows in ustreznih različicah strežnika.</span><span class="sxs-lookup"><span data-stu-id="a4388-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="a4388-108">Uporabniki z računi domene privzeto niso samodejno vpisani; Če želite omogočiti samodejno vpis, uporabite pravilnik **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="a4388-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="a4388-109">Če želite omogočiti samodejno vpis za uporabnike z računi Azure AD, razmislite o hibridnih pridruževanju svojih naprav.</span><span class="sxs-lookup"><span data-stu-id="a4388-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="a4388-110">**Privzeti račun za OS je Microsoftov račun**: Ta možnost je na voljo v sistemu Windows 10 RS3 (različica 1709, graditev 10.0.16299) in novejših različicah.</span><span class="sxs-lookup"><span data-stu-id="a4388-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="a4388-111">V napravah za podjetja ni verjetno, da bi prišlo do scenarija.</span><span class="sxs-lookup"><span data-stu-id="a4388-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="a4388-112">Če pa je privzeti račun za OS Microsoftov račun, se Microsoft Edge samodejno vpiše v uporabnika z Microsoftovim računom.</span><span class="sxs-lookup"><span data-stu-id="a4388-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
