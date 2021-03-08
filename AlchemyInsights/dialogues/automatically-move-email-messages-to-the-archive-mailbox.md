---
title: Samodejno premikanje e-poštnih sporočil v nabiralnik arhiva
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527099"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="2dac6-102">Samodejno premikanje e-poštnih sporočil v nabiralnik arhiva</span><span class="sxs-lookup"><span data-stu-id="2dac6-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="2dac6-103">Navodila za nastavitev pravilnika za samodejno premikanje stare e-pošte uporabnikov v arhivski nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="2dac6-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="2dac6-104">Če želite [](https://go.microsoft.com/fwlink/p/?linkid=2077143)preveriti, ali je  >    >  bil za uporabnika omogočen arhivski nabiralnik, se po&te v **arhivu** za upravljanje podatkov o skladnosti.</span><span class="sxs-lookup"><span data-stu-id="2dac6-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="2dac6-105">Če ni, kliknite **Omogoči** nato **da** v polju z opozorilom.</span><span class="sxs-lookup"><span data-stu-id="2dac6-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="2dac6-106">Pojdite v [**skrbniško središče za Exchange > upravljanje ustreznosti > oznak za hranjenje**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="2dac6-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="2dac6-107">Izberite ikono +, nato pa izberite **samodejno uporabi za celoten nabiralnik**.</span><span class="sxs-lookup"><span data-stu-id="2dac6-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="2dac6-108">Dodelite ime oznaki za hranjenje in izberite **Premakni v Arhiv**.</span><span class="sxs-lookup"><span data-stu-id="2dac6-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="2dac6-109">Za obdobje hranjenja vnesite želeni čas, na primer 90 dni.</span><span class="sxs-lookup"><span data-stu-id="2dac6-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="2dac6-110">Kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="2dac6-110">Click **Save**.</span></span>
5. <span data-ttu-id="2dac6-111">Zdaj ustvarite pravilnik o hranjenju: izberite **Pravilniki o hranjenju**, izberite ikono za dodajanje novega pravilnika.</span><span class="sxs-lookup"><span data-stu-id="2dac6-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="2dac6-112">Dodelite ime pravilniku o hranjenju, nato pa kliknite in se pomaknite, da poiščete in dodate oznako hranjenja, ki ste jo pravkar ustvarili.</span><span class="sxs-lookup"><span data-stu-id="2dac6-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="2dac6-113">Kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="2dac6-113">Click **Save**.</span></span>
7. <span data-ttu-id="2dac6-114">Na koncu uporabite pravilnik o hranjenju v nabiralniku uporabnika: še vedno v skrbniškem središču za Exchange odprite   >  **nabiralnike** prejemnikov.</span><span class="sxs-lookup"><span data-stu-id="2dac6-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="2dac6-115">Izberite vse uporabnike, za katere želite uporabiti pravilnik, nato pa izberite **Uredi** (ikona svinčnika).</span><span class="sxs-lookup"><span data-stu-id="2dac6-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="2dac6-116">V pogovornem oknu kliknite **funkcije nabiralnika**.</span><span class="sxs-lookup"><span data-stu-id="2dac6-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="2dac6-117">V razdelku **pravilnik o hranjenju** uporabite pravilnik, ki ste ga pravkar ustvarili > **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="2dac6-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="2dac6-118">Če želite navodila za uporabo pravilnika za vse uporabnike, glejte [Uporaba pravilnika o hranjenju za nabiralnike](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="2dac6-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
