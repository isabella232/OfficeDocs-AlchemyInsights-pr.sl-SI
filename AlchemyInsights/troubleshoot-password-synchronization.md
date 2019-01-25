---
title: Odpravljanje težav s sinhronizacijo geslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489952"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="466fa-102">Odpravljanje težav s sinhronizacijo geslo</span><span class="sxs-lookup"><span data-stu-id="466fa-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="466fa-103">Za odpravljanje težav, kjer brez gesla so sinhronizirani z Azure AD povezavo različico 1.1.614.0 ali novejšo različico:</span><span class="sxs-lookup"><span data-stu-id="466fa-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="466fa-104">Odprite novo sejo lupine Windows PowerShell na strežniku Azure AD povezavo s **prost dostop kot oskrbnik** predkupna pravica.</span><span class="sxs-lookup"><span data-stu-id="466fa-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="466fa-105">Teči **niz-pravilnika o izvajanju lupine RemoteSigned** ali **niz-pravilnika o izvajanju lupine neomejen**.</span><span class="sxs-lookup"><span data-stu-id="466fa-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="466fa-106">Zagnati čarovnika Azure AD povezavo.</span><span class="sxs-lookup"><span data-stu-id="466fa-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="466fa-107">Pluti v \*\* dodatne naloge \*\* strani, izberite \*\* odpravljanje \*\*, in kliknite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="466fa-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="466fa-108">Na strani odpravljanje težav, kliknite meni **začetek za začetek odpravljanja napak** v lupini PowerShell.</span><span class="sxs-lookup"><span data-stu-id="466fa-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="466fa-109">V glavnem meniju, izberite **Odpravljanje težav s sinhronizacijo geslo**.</span><span class="sxs-lookup"><span data-stu-id="466fa-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="466fa-110">V podmeniju, izberite **sinhronizacijo geslo ne dela na vseh**.</span><span class="sxs-lookup"><span data-stu-id="466fa-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="466fa-111">**Spoznajo rezultate opravila, odpravljanje težav**</span><span class="sxs-lookup"><span data-stu-id="466fa-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="466fa-112">Odpravljanje težav nalogo opravlja naslednje preglede:</span><span class="sxs-lookup"><span data-stu-id="466fa-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="466fa-113">Potrjuje, da je geslo sinhronizacijo možnost omogočena za modro AD najemnik.</span><span class="sxs-lookup"><span data-stu-id="466fa-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="466fa-114">Potrjuje, da Azure AD Connect strežnikom ni v produkcijskem načinu.</span><span class="sxs-lookup"><span data-stu-id="466fa-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="466fa-115">Za vsak obstoječi krajevni Active Directory priključek (kar ustreza obstoječemu gozdu Active Directory):</span><span class="sxs-lookup"><span data-stu-id="466fa-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="466fa-116">Potrjuje, da je omogočena funkcija za sinhronizacijo geslo.</span><span class="sxs-lookup"><span data-stu-id="466fa-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="466fa-117">Išče geslo sinhronizacijo srčni utrip dogodkov v dnevnikih dogodkov za program Windows.</span><span class="sxs-lookup"><span data-stu-id="466fa-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="466fa-118">Za vsako domeno Active Directory pod priključek krajevnega imenika Active Directory:</span><span class="sxs-lookup"><span data-stu-id="466fa-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="466fa-119">Potrjuje, da je dosegljiv iz Azure AD povezavo strežnika domene.</span><span class="sxs-lookup"><span data-stu-id="466fa-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="466fa-120">Potrjuje, da domene storitve Active Directory (AD DS) kontov, s krajevnim Active Directory priključek je pravilno uporabniško ime, geslo in dovoljenja, zahtevana za sinhronizacijo geslo.</span><span class="sxs-lookup"><span data-stu-id="466fa-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="466fa-121">Pomoč parola omedlevičen za odpravljanje težav, glejte [Odpravljanje geslo sinhronizacije z Azure AD povezavo sinhronizacijo](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="466fa-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

