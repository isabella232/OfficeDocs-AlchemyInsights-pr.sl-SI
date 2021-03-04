---
title: Nadzorovanje pogojnega dostopa za InTune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428307"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="0d250-102">Nadzorovanje pogojnega dostopa za InTune</span><span class="sxs-lookup"><span data-stu-id="0d250-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="0d250-103">Uporabniki, ki so usmerjeni s pogojnim dostopom, bodo prejeli e-poštno obvestilo, če ne ustrezajo zahtevam za dostop do vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="0d250-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0d250-104">Če želite razrešiti, priporočamo eno ali več od teh rešitev:</span><span class="sxs-lookup"><span data-stu-id="0d250-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="0d250-105">Če je naprava domnevno včlanjena, svetuje uporabniku, da se poišče v programu podjetja portal in preveri, ali je prikazana v portalu podjetja.</span><span class="sxs-lookup"><span data-stu-id="0d250-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0d250-106">Če ne, mora uporabnik vpisati napravo.</span><span class="sxs-lookup"><span data-stu-id="0d250-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="0d250-107">V portalu **Azure se pozanimajte o**  >  **skladnosti naprave**.</span><span class="sxs-lookup"><span data-stu-id="0d250-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="0d250-108">Če si želite ogledati poročilo o skladnosti naprave, da preverite, ali je naprava uporabnika označena kot združljiva, v razdelku **monitor** kliknite **skladnost naprave**.</span><span class="sxs-lookup"><span data-stu-id="0d250-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="0d250-109">V portalu **Azure se pozanimajte o**  >  **skladnosti naprave**.</span><span class="sxs-lookup"><span data-stu-id="0d250-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="0d250-110">V razdelku **upravljanje** kliknite **Pravilniki**.</span><span class="sxs-lookup"><span data-stu-id="0d250-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="0d250-111">Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen napravi uporabnika.</span><span class="sxs-lookup"><span data-stu-id="0d250-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0d250-112">Če ni dodeljen noben profil, InTune ne more potrditi stanja skladnosti naprave.</span><span class="sxs-lookup"><span data-stu-id="0d250-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="0d250-113">Uredite uporabnikovo pogojno dostopno dodelitev.</span><span class="sxs-lookup"><span data-stu-id="0d250-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="0d250-114">V portalu Azure se pomaknite do možnosti **Prilagodi**  >  pravilnike **pogojnega dostopa**  >  , na seznamu izberite pravilnik in kliknite **Uporabniki in skupine**.</span><span class="sxs-lookup"><span data-stu-id="0d250-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="0d250-115">Če želite določene pravilnike usmeriti na osebo, jih dodajte na **seznam vključi**.</span><span class="sxs-lookup"><span data-stu-id="0d250-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="0d250-116">Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jih dodajte na **seznam izključi**.</span><span class="sxs-lookup"><span data-stu-id="0d250-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="0d250-117">**Uporabne povezave:**</span><span class="sxs-lookup"><span data-stu-id="0d250-117">**Helpful links:**</span></span>

- [<span data-ttu-id="0d250-118">Pregled skladnosti naprave</span><span class="sxs-lookup"><span data-stu-id="0d250-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="0d250-119">Odpravljanje težav CA</span><span class="sxs-lookup"><span data-stu-id="0d250-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="0d250-120">Pravilnik za odpravljanje težav</span><span class="sxs-lookup"><span data-stu-id="0d250-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="0d250-121">Nadzorovanje skladnosti naprave</span><span class="sxs-lookup"><span data-stu-id="0d250-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="0d250-122">Ti koraki so v pomoč pri odpravljanju težav s pogojnim dostopom v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d250-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="0d250-123">Možno je tudi, da karantena naprave blokira dostop do e-pošte s pravilnikom za Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d250-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="0d250-124">Več informacij o upravljanju naprav Exchange lahko najdete [**tukaj**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="0d250-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
