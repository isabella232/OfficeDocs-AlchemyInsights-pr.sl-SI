---
title: Popravi pravilnik povezave
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695888"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="dd100-102">Popravi pravilnik povezave</span><span class="sxs-lookup"><span data-stu-id="dd100-102">Fix connection policy</span></span>

<span data-ttu-id="dd100-103">E-pošta je bila označena kot varna in dostavljena v uporabnikovo mapo» Prejeto «, ker je bil naslov IP za pošiljanje v pravilniku filtra povezave označen kot varen.</span><span class="sxs-lookup"><span data-stu-id="dd100-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="dd100-104">Če želite pregledati pravilnik, naredite to:</span><span class="sxs-lookup"><span data-stu-id="dd100-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="dd100-105">Obiščite središče za [skladnost s predpisi sistema Office & 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)in nato pojdite na pravilnik za **upravljanje groženj** za  >    >  [preprečevanje neželene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="dd100-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="dd100-106">Na zavihku **po meri** izberite **pravilnik filtra povezave** in nato izberite **Uredi pravilnik**.</span><span class="sxs-lookup"><span data-stu-id="dd100-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="dd100-107">Preglejte seznam **dovoljenih IP** .</span><span class="sxs-lookup"><span data-stu-id="dd100-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="dd100-108">Preverite, ali je omogočen **varni seznam** .</span><span class="sxs-lookup"><span data-stu-id="dd100-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="dd100-109">Microsoft je naročen na vire neodvisnih ponudnikov zaupanja vrednih pošiljateljev.</span><span class="sxs-lookup"><span data-stu-id="dd100-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="dd100-110">Če je omogočeno **varno seznam** , se ti zaupanja vredni pošiljatelji ne zmotno označijo kot neželena pošta.</span><span class="sxs-lookup"><span data-stu-id="dd100-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="dd100-111">Priporočamo, da izberete to možnost, saj bo zmanjšala število lažnih pozitivnih rezultatov (dobra pošta, ki je razvrščena kot neželena pošta), ki jo prejmete.</span><span class="sxs-lookup"><span data-stu-id="dd100-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
