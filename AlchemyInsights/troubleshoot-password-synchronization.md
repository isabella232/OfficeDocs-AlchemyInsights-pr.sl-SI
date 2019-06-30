---
title: Odpravljanje težav s sinhronizacijo geslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353121"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c6f4a-102">Odpravljanje težav s sinhronizacijo geslo</span><span class="sxs-lookup"><span data-stu-id="c6f4a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c6f4a-103">Za odpravljanje težav, kjer brez gesla so sinhronizirani z Azure AD povezavo različico 1.1.614.0 ali novejšo različico:</span><span class="sxs-lookup"><span data-stu-id="c6f4a-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="c6f4a-104">Odprite novo sejo lupine Windows PowerShell na strežniku Azure AD povezavo s **prost dostop kot oskrbnik** predkupna pravica.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c6f4a-105">Teči **niz-pravilnika o izvajanju lupine RemoteSigned** ali **niz-pravilnika o izvajanju lupine neomejen**.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="c6f4a-106">Zagnati čarovnika Azure AD povezavo.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c6f4a-107">Pojdite na **Dodatne naloge** , izberite **Odpravljanje težav**in kliknite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="c6f4a-108">Na strani odpravljanje težav, kliknite meni **začetek za začetek odpravljanja napak** v lupini PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="c6f4a-109">V glavnem meniju, izberite **Odpravljanje težav s sinhronizacijo geslo**.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="c6f4a-110">V podmeniju, izberite **sinhronizacijo geslo ne dela na vseh**.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="c6f4a-111">**Spoznajo rezultate opravila, odpravljanje težav**</span><span class="sxs-lookup"><span data-stu-id="c6f4a-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="c6f4a-112">Odpravljanje težav nalogo opravlja naslednje preglede:</span><span class="sxs-lookup"><span data-stu-id="c6f4a-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="c6f4a-113">Potrjuje, da je geslo sinhronizacijo možnost omogočena za modro AD najemnik.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="c6f4a-114">Potrjuje, da Azure AD Connect strežnikom ni v produkcijskem načinu.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="c6f4a-115">Za vsak obstoječi krajevni Active Directory priključek (kar ustreza obstoječemu gozdu Active Directory):</span><span class="sxs-lookup"><span data-stu-id="c6f4a-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="c6f4a-116">Potrjuje, da je omogočena funkcija za sinhronizacijo geslo.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="c6f4a-117">Išče geslo sinhronizacijo srčni utrip dogodkov v dnevnikih dogodkov za program Windows.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="c6f4a-118">Za vsako domeno Active Directory pod priključek krajevnega imenika Active Directory:</span><span class="sxs-lookup"><span data-stu-id="c6f4a-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="c6f4a-119">Potrjuje, da je dosegljiv iz Azure AD povezavo strežnika domene.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="c6f4a-120">Potrjuje, da domene storitve Active Directory (AD DS) kontov, s krajevnim Active Directory priključek je pravilno uporabniško ime, geslo in dovoljenja, zahtevana za sinhronizacijo geslo.</span><span class="sxs-lookup"><span data-stu-id="c6f4a-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="c6f4a-121">Pomoč parola omedlevičen za odpravljanje težav, glejte [Odpravljanje geslo sinhronizacije z Azure AD povezavo sinhronizacijo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c6f4a-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  