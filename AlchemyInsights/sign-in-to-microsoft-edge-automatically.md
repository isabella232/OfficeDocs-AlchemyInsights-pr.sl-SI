---
title: Samodejni vpis v Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398745"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="f0283-102">Samodejni vpis v Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f0283-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="f0283-103">Microsoft Edge s privzetim računom operacijskega sistema samodejno vpiše uporabnika glede na to, kako je konfigurirana uporabnikova naprava.</span><span class="sxs-lookup"><span data-stu-id="f0283-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="f0283-104">Scenariji posamezne vrste konfiguracije naprave in odvisni procesi vpisa uporabnikov so opisani spodaj:</span><span class="sxs-lookup"><span data-stu-id="f0283-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="f0283-105">**Naprava je hibridna/AAD-J:** Ta možnost je na voljo v sistemu Windows 10, sistemih Windows navzdol in ustreznih različicah strežnika.</span><span class="sxs-lookup"><span data-stu-id="f0283-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="f0283-106">Uporabniki so samodejno vpisani s svojimi računi imenika Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="f0283-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="f0283-107">**Naprava je pridružena domeni:** Ta možnost je na voljo v sistemu Windows 10, sistemu Windows s ravneh navzdol in ustreznih različicah strežnika.</span><span class="sxs-lookup"><span data-stu-id="f0283-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="f0283-108">Uporabniki z računi domene privzeto niso vpisani samodejno; če želite omogočiti samodejni vpis zanje, uporabite pravilnik **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="f0283-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="f0283-109">Če želite omogočiti samodejni vpis za uporabnike z računi Azure AD, razmislite o hibridnem pridruževati se svojim napravam.</span><span class="sxs-lookup"><span data-stu-id="f0283-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="f0283-110">Privzeti **račun operacijskega** sistema je Microsoftov račun: ta možnost je na voljo v sistemu Windows 10 RS3 (različica 1709, gradjša 10.0.16299) in novejših različicah.</span><span class="sxs-lookup"><span data-stu-id="f0283-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="f0283-111">Ta scenarij je malo verjeten za uporabo v napravah podjetja.</span><span class="sxs-lookup"><span data-stu-id="f0283-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="f0283-112">Če pa je privzeti račun operacijskega sistema Microsoftov račun, se microsoft Edge samodejno vpiše z uporabnikom z Microsoftovim računom.</span><span class="sxs-lookup"><span data-stu-id="f0283-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
