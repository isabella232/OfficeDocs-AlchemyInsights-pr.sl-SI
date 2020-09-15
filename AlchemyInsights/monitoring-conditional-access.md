---
title: Nadzorovanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702919"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="9ef27-102">Nadzorovanje pogojnega dostopa za Exchange</span><span class="sxs-lookup"><span data-stu-id="9ef27-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="9ef27-103">Uporabniki, ki so usmerjeni s pogojnim dostopom, bodo prejeli e-poštno obvestilo, če ne ustrezajo zahtevam za dostop do vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="9ef27-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9ef27-104">Če želite razrešiti, priporočamo eno ali več od teh rešitev:</span><span class="sxs-lookup"><span data-stu-id="9ef27-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="9ef27-105">Če je naprava domnevno včlanjena, svetuje uporabniku, da se poišče v programu podjetja portal in preveri, ali je prikazana v portalu podjetja.</span><span class="sxs-lookup"><span data-stu-id="9ef27-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9ef27-106">Če ne, mora uporabnik vpisati napravo.</span><span class="sxs-lookup"><span data-stu-id="9ef27-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="9ef27-107">V portalu Azure se pozanimajte o \*\* \> skladnosti naprave\*\*.</span><span class="sxs-lookup"><span data-stu-id="9ef27-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="9ef27-108">V razdelku **monitor** kliknite **skladnost naprave**.</span><span class="sxs-lookup"><span data-stu-id="9ef27-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="9ef27-109">Če želite preveriti, ali je naprava uporabnika označena kot združljiva, si oglejte poročilo o skladnosti naprave.</span><span class="sxs-lookup"><span data-stu-id="9ef27-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="9ef27-110">V portalu Azure se pozanimajte o \*\* \> skladnosti naprave\*\*.</span><span class="sxs-lookup"><span data-stu-id="9ef27-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="9ef27-111">V razdelku **upravljanje**kliknite **Pravilniki**.</span><span class="sxs-lookup"><span data-stu-id="9ef27-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="9ef27-112">Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen napravi uporabnika.</span><span class="sxs-lookup"><span data-stu-id="9ef27-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9ef27-113">Če ni dodeljen noben profil, InTune ne more potrditi stanja skladnosti naprave.</span><span class="sxs-lookup"><span data-stu-id="9ef27-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="9ef27-114">Uredite uporabnikovo pogojno dostopno dodelitev.</span><span class="sxs-lookup"><span data-stu-id="9ef27-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="9ef27-115">V portalu Azure se pozanimajte za **InTune \> \> pravilnika za pogojni dostop**</span><span class="sxs-lookup"><span data-stu-id="9ef27-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="9ef27-116">Izbira pravilnika s seznama</span><span class="sxs-lookup"><span data-stu-id="9ef27-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="9ef27-117">Kliknite **Uporabniki in skupine**</span><span class="sxs-lookup"><span data-stu-id="9ef27-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="9ef27-118">Če želite določene pravilnike usmeriti na osebo, jih dodajte na seznam **vključi** .</span><span class="sxs-lookup"><span data-stu-id="9ef27-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="9ef27-119">Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jih dodajte na seznam **izključi** .</span><span class="sxs-lookup"><span data-stu-id="9ef27-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="9ef27-120">Preberite več [o tem: Kako spremljati naprave s pogojnim dostopom](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="9ef27-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

