---
title: Spremljanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656583"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="13807-102">Spremljanje pogojnega dostopa</span><span class="sxs-lookup"><span data-stu-id="13807-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="13807-p101">Uporabniki, ki so usmerjena s pogojnim dostopom prejmejo oznanilo email, če izpolnjuje zahteve vaše organizacije. Odločiti, priporočamo, da eden ali več od naslednjih rešitev:</span><span class="sxs-lookup"><span data-stu-id="13807-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="13807-p102">Če naprava je domneva, da bodo vpisani, svetuje uporabnik iti podjetje Portal app in preveri, da se pojavi v portalu podjetja. Če ne, uporabnik vpisati naprave.</span><span class="sxs-lookup"><span data-stu-id="13807-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="13807-p103">V portalu Azure iti **Intune \> skladnost naprave**. Pod **oknom** kliknite **napravo skladnosti**. Poglej si poročilo skladnost naprave za preverjanje, da uporabnikova naprava je označena kot skladna.</span><span class="sxs-lookup"><span data-stu-id="13807-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="13807-p104">V portalu Azure iti **Intune \> skladnost naprave**. Pod **upravljanje**, kliknite **pravila**. Na seznamu skladnost politik, preverite, ali da je dodeljen profil vaš uporabnik naprave. Če je dodeljena brez profila, Intune ne bo zmožen potrditi skladnost stanje naprave.</span><span class="sxs-lookup"><span data-stu-id="13807-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="13807-114">Urejanje dodelitev pogojnega dostopa uporabnika.</span><span class="sxs-lookup"><span data-stu-id="13807-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="13807-115">V portalu Azure iti **Intune \> pogojni dostop \> pravila**</span><span class="sxs-lookup"><span data-stu-id="13807-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="13807-116">Na seznamu izberite politike</span><span class="sxs-lookup"><span data-stu-id="13807-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="13807-117">Kliknite **Uporabniki in skupine**</span><span class="sxs-lookup"><span data-stu-id="13807-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="13807-p105">Cilj politike na nekoga, jih dodajte na seznam **vključitev** . Če želite zagotoviti, da oseba izpustite iz pravilnika, dodati na seznam **izključitev** .</span><span class="sxs-lookup"><span data-stu-id="13807-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="13807-120">Preberite več: [Kako Monitor pogojnem dostopu naprave](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="13807-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

