---
title: Spremljanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713734"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="ce287-102">Spremljanje pogojnega dostopa za Exchange</span><span class="sxs-lookup"><span data-stu-id="ce287-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="ce287-103">Uporabniki, usmerjeni s pogojnim dostopom, prejmejo e-poštno sporočilo z obvestilom, če ne izpolnjujejo zahtev za dostop vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="ce287-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ce287-104">Za rešitev priporočamo eno ali več naslednjih rešitev:</span><span class="sxs-lookup"><span data-stu-id="ce287-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="ce287-105">Če se domneva, da je naprava vpisana v program, Svetujte uporabniku, da gre v aplikacijo portal podjetja, in preverite, ali je v portalu podjetja.</span><span class="sxs-lookup"><span data-stu-id="ce287-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ce287-106">Če se ne, mora uporabnik vpisati napravo.</span><span class="sxs-lookup"><span data-stu-id="ce287-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="ce287-107">V portalu Azure pojdite na \*\* \> prilagajanje skladnosti naprave\*\*.</span><span class="sxs-lookup"><span data-stu-id="ce287-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="ce287-108">Pod **monitor** kliknite **skladnost naprave**.</span><span class="sxs-lookup"><span data-stu-id="ce287-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="ce287-109">Oglejte si poročilo o skladnosti naprave, da preverite, ali je uporabniška naprava označena kot skladna.</span><span class="sxs-lookup"><span data-stu-id="ce287-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="ce287-110">V portalu Azure pojdite na \*\* \> prilagajanje skladnosti naprave\*\*.</span><span class="sxs-lookup"><span data-stu-id="ce287-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="ce287-111">V razdelku **upravljanje**kliknite **Pravilniki**.</span><span class="sxs-lookup"><span data-stu-id="ce287-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="ce287-112">Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen uporabnikovi napravi.</span><span class="sxs-lookup"><span data-stu-id="ce287-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ce287-113">Če profil ni dodeljen, InTune ne bo mogel potrditi stanja skladnosti naprave.</span><span class="sxs-lookup"><span data-stu-id="ce287-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="ce287-114">Uredite uporabniški nalog za pogojni dostop.</span><span class="sxs-lookup"><span data-stu-id="ce287-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="ce287-115">V portalu Azure pojdite na **InTune \> pravilniki pogojnega \> dostopa**</span><span class="sxs-lookup"><span data-stu-id="ce287-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="ce287-116">Izbiranje pravilnika s seznama</span><span class="sxs-lookup"><span data-stu-id="ce287-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="ce287-117">Kliknite **Uporabniki in skupine**</span><span class="sxs-lookup"><span data-stu-id="ce287-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="ce287-118">Če želite na nekoga ciljati določeno politiko, jih dodajte na seznam **vključi** .</span><span class="sxs-lookup"><span data-stu-id="ce287-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="ce287-119">Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jo dodajte na seznam **izključitev** .</span><span class="sxs-lookup"><span data-stu-id="ce287-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="ce287-120">Preberite več: [kako nadzorovati naprave s pogojnim dostopom](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="ce287-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

