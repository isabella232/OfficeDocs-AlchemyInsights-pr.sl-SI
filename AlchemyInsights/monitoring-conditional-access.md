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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708690"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="7e4ee-102">Nadzorovanje pogojnega dostopa za Exchange</span><span class="sxs-lookup"><span data-stu-id="7e4ee-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="7e4ee-103">Uporabniki, ki so usmerjeni s pogojnim dostopom, bodo prejeli e-poštno obvestilo, če ne ustrezajo zahtevam za dostop do vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7e4ee-104">Če želite razrešiti, priporočamo eno ali več od teh rešitev:</span><span class="sxs-lookup"><span data-stu-id="7e4ee-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="7e4ee-105">Če je naprava domnevno včlanjena, svetuje uporabniku, da se poišče v programu podjetja portal in preveri, ali je prikazana v portalu podjetja.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7e4ee-106">Če ne, mora uporabnik vpisati napravo.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="7e4ee-107">V portalu Azure obiščite spletno mesto InTune > skladnost z napravo.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="7e4ee-108">V razdelku monitor kliknite skladnost naprave.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="7e4ee-109">Če želite preveriti, ali je naprava uporabnika označena kot združljiva, si oglejte poročilo o skladnosti naprave.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="7e4ee-110">V portalu Azure obiščite spletno mesto InTune > skladnost z napravo.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="7e4ee-111">V razdelku upravljanje kliknite pravilniki.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-111">Under Manage, click Policies.</span></span> <span data-ttu-id="7e4ee-112">Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen napravi uporabnika.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7e4ee-113">Če ni dodeljen noben profil, InTune ne more potrditi stanja skladnosti naprave.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="7e4ee-114">Uredite uporabnikovo pogojno dostopno dodelitev.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="7e4ee-115">V portalu Azure se pozanimajte za **Nastavitev**  >  pravilnikov **pogojnega dostopa**  >  .</span><span class="sxs-lookup"><span data-stu-id="7e4ee-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="7e4ee-116">Na seznamu izberite pravilnik.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="7e4ee-117">Kliknite Uporabniki in skupine.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-117">Click Users and groups.</span></span>
4. <span data-ttu-id="7e4ee-118">Če želite določene pravilnike usmeriti na osebo, jih dodajte na seznam vključi.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="7e4ee-119">Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jih dodajte na seznam izključi.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="7e4ee-120">Uporabne povezave:</span><span class="sxs-lookup"><span data-stu-id="7e4ee-120">Helpful links:</span></span>

[<span data-ttu-id="7e4ee-121">Pregled skladnosti naprave</span><span class="sxs-lookup"><span data-stu-id="7e4ee-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="7e4ee-122">Odpravljanje težav CA</span><span class="sxs-lookup"><span data-stu-id="7e4ee-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7e4ee-123">Pravilnik za odpravljanje težav</span><span class="sxs-lookup"><span data-stu-id="7e4ee-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="7e4ee-124">Nadzorovanje skladnosti naprave</span><span class="sxs-lookup"><span data-stu-id="7e4ee-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="7e4ee-125">Opomba: ta navodila so koristna le za odpravljanje težav s pogojnim dostopom v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="7e4ee-126">Možno je tudi, da karantena naprave blokira dostop do e-pošte s pravilnikom za Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e4ee-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="7e4ee-127">Več informacij o upravljanju Exchangeeve naprave lahko najdete [tukaj] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="7e4ee-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
