---
title: Spremljanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418485"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="dbce5-102">Spremljanje pogojnega dostopa</span><span class="sxs-lookup"><span data-stu-id="dbce5-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="dbce5-103">Uporabniki, ki so usmerjena s pogojnim dostopom prejmejo oznanilo email, če izpolnjuje zahteve vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="dbce5-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="dbce5-104">Odločiti, priporočamo, da eden ali več od naslednjih rešitev:</span><span class="sxs-lookup"><span data-stu-id="dbce5-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="dbce5-105">Če naprava je domneva, da bodo vpisani, svetuje uporabnik iti podjetje Portal app in preveri, da se pojavi v portalu podjetja.</span><span class="sxs-lookup"><span data-stu-id="dbce5-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="dbce5-106">Če ne, uporabnik vpisati naprave.</span><span class="sxs-lookup"><span data-stu-id="dbce5-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="dbce5-107">V portalu Azure iti **Intune \> skladnost naprave**.</span><span class="sxs-lookup"><span data-stu-id="dbce5-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="dbce5-108">Pod **oknom** kliknite **napravo skladnosti**.</span><span class="sxs-lookup"><span data-stu-id="dbce5-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="dbce5-109">Poglej si poročilo skladnost naprave za preverjanje, da uporabnikova naprava je označena kot skladna.</span><span class="sxs-lookup"><span data-stu-id="dbce5-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="dbce5-110">V portalu Azure iti **Intune \> skladnost naprave**.</span><span class="sxs-lookup"><span data-stu-id="dbce5-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="dbce5-111">Pod **upravljanje**, kliknite **pravila**.</span><span class="sxs-lookup"><span data-stu-id="dbce5-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="dbce5-112">Na seznamu skladnost politik, preverite, ali da je dodeljen profil vaš uporabnik naprave.</span><span class="sxs-lookup"><span data-stu-id="dbce5-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="dbce5-113">Če je dodeljena brez profila, Intune ne bo zmožen potrditi skladnost stanje naprave.</span><span class="sxs-lookup"><span data-stu-id="dbce5-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="dbce5-114">Urejanje dodelitev pogojnega dostopa uporabnika.</span><span class="sxs-lookup"><span data-stu-id="dbce5-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="dbce5-115">V portalu Azure iti **Intune \> pogojni dostop \> pravila**</span><span class="sxs-lookup"><span data-stu-id="dbce5-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="dbce5-116">Na seznamu izberite politike</span><span class="sxs-lookup"><span data-stu-id="dbce5-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="dbce5-117">Kliknite **Uporabniki in skupine**</span><span class="sxs-lookup"><span data-stu-id="dbce5-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="dbce5-118">Cilj politike na nekoga, jih dodajte na seznam **vključitev** .</span><span class="sxs-lookup"><span data-stu-id="dbce5-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="dbce5-119">Če želite zagotoviti, da oseba izpustite iz pravilnika, dodati na seznam **izključitev** .</span><span class="sxs-lookup"><span data-stu-id="dbce5-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="dbce5-120">Preberite več: [Kako Monitor pogojnem dostopu naprave](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="dbce5-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

