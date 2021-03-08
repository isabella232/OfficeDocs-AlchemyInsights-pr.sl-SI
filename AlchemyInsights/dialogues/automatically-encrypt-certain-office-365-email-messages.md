---
title: Samodejno šifriranje določenih e-poštnih sporočil sistema Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526742"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="3a6ab-102">Samodejno šifriranje določenih e-poštnih sporočil sistema Office 365</span><span class="sxs-lookup"><span data-stu-id="3a6ab-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="3a6ab-103">Samodejno lahko šifrirate sporočila, ki jih uporabniki pošiljajo določenim zunanjim osebam ali organizacijam.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="3a6ab-104">To naredite tako, da izvedete te korake:</span><span class="sxs-lookup"><span data-stu-id="3a6ab-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="3a6ab-105">V [skrbniškem središču za Exchange](https://outlook.office365.com/ecp/)izberite **pravila toka pošte >**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="3a6ab-106">Kliknite ikono **novo (+)** , nato pa kliknite **uporabi šifriranje sporočil sistema Office 365 in zaščito pravic za sporočila**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="3a6ab-107">V polje **ime** vnesite ime za pravilo, na primer *šifriranje sporočil, poslanih v DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="3a6ab-108">**Če želite uporabiti to pravilo, če** izberite **prejemnik > je ta oseba**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="3a6ab-109">V oknu **Izberite člane** izberite ime osebe, za katero želite uporabiti pravilo šifriranja, in nato kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="3a6ab-110">Ko končate Dodajanje uporabnikov, kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="3a6ab-111">Poleg polja **naredi to** kliknite **Izberi eno**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="3a6ab-112">V spustnem meniju **predloga RMS** izberite **Šifriraj** in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="3a6ab-113">(Če ne vidite te možnosti, to pomeni, da vaš paket ne vključuje samodejnega šifriranja.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="3a6ab-114">Vendar ga lahko dodate!)</span><span class="sxs-lookup"><span data-stu-id="3a6ab-114">But you can add it!)</span></span>
9. <span data-ttu-id="3a6ab-115">Izberite poljuben izbirni izbor (na seznamu izbirnih izbir, ki jih lahko naredite na tej strani, od katerih jih je mogoče preprostiti s privzeto nastavitev za enostavnost).</span><span class="sxs-lookup"><span data-stu-id="3a6ab-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="3a6ab-116">Kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3a6ab-117">Pozneje se lahko vrnete in uredite to pravilo.</span><span class="sxs-lookup"><span data-stu-id="3a6ab-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="3a6ab-118">Če želite več informacij o ustvarjanju pravil za šifriranje, glejte [določanje pravil pretoka pošte za šifriranje e-poštnih sporočil v storitvi Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="3a6ab-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

