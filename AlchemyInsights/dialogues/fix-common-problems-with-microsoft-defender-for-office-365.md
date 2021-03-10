---
title: Odpravljanje pogostih težav s storitvijo Microsoft Defender za Office 365
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
- "9000760"
- "7391"
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695628"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="ed072-102">Odpravljanje pogostih težav s storitvijo Microsoft Defender za Office 365</span><span class="sxs-lookup"><span data-stu-id="ed072-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="ed072-103">Tukaj je nekaj rešitev za pogoste težave s storitvijo Microsoft Defender za Office 365:</span><span class="sxs-lookup"><span data-stu-id="ed072-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="ed072-104">**Zakasnitev sporočila:** Če imate težave z zakasnitvijo dostave sporočila, boste želeli uporabiti **dinamične možnosti dostave** v pravilniku o varnih prilogah.</span><span class="sxs-lookup"><span data-stu-id="ed072-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="ed072-105">Če želite več informacij, glejte [dinamična dostava v pravilnikih varnih prilog](https://go.microsoft.com/fwlink/?linkid=2094106).</span><span class="sxs-lookup"><span data-stu-id="ed072-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="ed072-106">**Prijavite lažne pozitivne ali negativne rezultate:** Prijavite sporočilo Microsoftu s to povezavo: portal za [odzive Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2092835).</span><span class="sxs-lookup"><span data-stu-id="ed072-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="ed072-107">**Omogoči zaščito varne povezave:**</span><span class="sxs-lookup"><span data-stu-id="ed072-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="ed072-108">Vpišite se v [središče za skladnost z varnostnim &om sistema Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="ed072-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="ed072-109">Pojdite na   >    >  **varna povezava** pravilnika za upravljanje groženj.</span><span class="sxs-lookup"><span data-stu-id="ed072-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="ed072-110">V razdelku **pravilniki, ki veljajo za določene prejemnike**, odprite konfiguriran pravilnik.</span><span class="sxs-lookup"><span data-stu-id="ed072-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="ed072-111">V razdelku **Nastavitve** izberite **uporabi varne povezave do sporočil, ki so poslana v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="ed072-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
