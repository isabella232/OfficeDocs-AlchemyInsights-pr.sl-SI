---
title: Odpravljanje težav s sinhronizacijo gesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387893"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="fa2e9-102">Odpravljanje težav s sinhronizacijo gesel</span><span class="sxs-lookup"><span data-stu-id="fa2e9-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="fa2e9-103">Če želite odpraviti težave s sinhronizacijo gesel, začnite z opravilom za odpravljanje težav aAD Connect, da ugotovite, zakaj se gesla ne sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="fa2e9-104">Če želite začeti, pojdite [na Upravljanje neposredne sinhronizacije](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="fa2e9-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="fa2e9-105">Odprite novo sejo lupine Windows PowerShell v strežniku Azure AD Connect in izberite možnost **Zaženi kot** skrbnik.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="fa2e9-106">Zaženite RemoteSigned Set-ExecutionPolicy ali Set-ExecutionPolicy neomejeno.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="fa2e9-107">Zaženite čarovnika za povezavo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="fa2e9-108">Pojdite na stran Dodatna opravila > **Odpravljanje**  >  **težav .**</span><span class="sxs-lookup"><span data-stu-id="fa2e9-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="fa2e9-109">Izberite **Zaženi,** da odprete meni za odpravljanje težav z Lupino PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="fa2e9-110">Izberite **Odpravljanje težav s sinhronizacijo gesel**.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="fa2e9-111">Težava je po navadi, da geslo ni sinhronizirano za določen uporabniški račun.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="fa2e9-112">**Opombe** Sinhronizacija gesel ne uspe, če je bila zadnja uspešna sinhronizacija gesel pred časom.</span><span class="sxs-lookup"><span data-stu-id="fa2e9-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="fa2e9-113">Če želite več pomoči pri odpravljanju težav s sinhronizacijo gesel, glejte Odpravljanje težav s sinhronizacijo z [razhajanjem gesel s sinhronizacijo storitve Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="fa2e9-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>