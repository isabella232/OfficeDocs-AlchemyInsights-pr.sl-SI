---
title: Odpravljanje težav pri sinhronizaciji gesel
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732526"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e8651-102">Odpravljanje težav pri sinhronizaciji gesel</span><span class="sxs-lookup"><span data-stu-id="e8651-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e8651-103">Če želite odpraviti težave, pri katerih se gesla ne sinhronizirajo s storitvijo Azure AD Connect 1.1.614.0 ali novejšo različico:</span><span class="sxs-lookup"><span data-stu-id="e8651-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="e8651-104">Odprite novo sejo lupine Windows PowerShell v strežniku Azure AD Connect z možnostjo **Zaženi kot skrbnik** .</span><span class="sxs-lookup"><span data-stu-id="e8651-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e8651-105">Zaženi **nastavljeno-ExecutionPolicy Remotepodpisano** ali **nastavljeno-ExecutionPolicy neomejen**.</span><span class="sxs-lookup"><span data-stu-id="e8651-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="e8651-106">Zaženite čarovnika za povezavo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e8651-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e8651-107">Pomaknite se na stran **dodatna opravila** , izberite **Odpravljanje težav**in kliknite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="e8651-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="e8651-108">Na strani za odpravljanje težav kliknite **Zaženi, da zaženete meni za odpravljanje težav** v PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e8651-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="e8651-109">V glavnem meniju izberite **Odpravljanje težav s sinhronizacijo gesel**.</span><span class="sxs-lookup"><span data-stu-id="e8651-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="e8651-110">V podmeniju izberite **sinhronizacija gesel sploh ne deluje**.</span><span class="sxs-lookup"><span data-stu-id="e8651-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="e8651-111">**Razumevanje rezultatov opravila za odpravljanje težav**</span><span class="sxs-lookup"><span data-stu-id="e8651-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="e8651-112">Opravilo za odpravljanje težav izvede te preglede:</span><span class="sxs-lookup"><span data-stu-id="e8651-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="e8651-113">Potrdi, da je funkcija sinhronizacije gesel omogočena za najemnika Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e8651-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="e8651-114">Potrdi, da strežnik Azure AD Connect ni v načinu Stopnjevitost.</span><span class="sxs-lookup"><span data-stu-id="e8651-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="e8651-115">Za vsak obstoječi krajevni konektor imenika Active Directory (ki ustreza obstoječemu gozdu imenika Active Directory):</span><span class="sxs-lookup"><span data-stu-id="e8651-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="e8651-116">Potrdi, da je funkcija sinhronizacije gesel omogočena.</span><span class="sxs-lookup"><span data-stu-id="e8651-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="e8651-117">Poišče dogodke srčnega utripa za sinhronizacijo gesel v dnevnikih programa Windows Application Event.</span><span class="sxs-lookup"><span data-stu-id="e8651-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="e8651-118">Za vsako domeno imenika Active Directory pod krajevnim konektorjem imenika Active Directory:</span><span class="sxs-lookup"><span data-stu-id="e8651-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="e8651-119">Preveri, ali je domena dosegljiva iz strežnika Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e8651-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="e8651-120">Preveri, ali so računi storitve Active Directory (AD DS), ki jih uporablja krajevni konektor imenika Active Directory, pravilno uporabniško ime, geslo in dovoljenja, potrebna za sinhronizacijo gesel.</span><span class="sxs-lookup"><span data-stu-id="e8651-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="e8651-121">Če želite več pomoči pri sinhronizaciji gesel, glejte [Odpravljanje težav s sinhronizacijo gesel s sinhronizacijo AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e8651-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  