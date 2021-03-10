---
title: Popravi pravilnik najemnika (preglasitev dejanja)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695693"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="69a5f-102">Popravi pravilnik najemnika (preglasitev dejanja)</span><span class="sxs-lookup"><span data-stu-id="69a5f-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="69a5f-103">To sporočilo je vplivalo na pravilnik proti neželene pošte v najemniku.</span><span class="sxs-lookup"><span data-stu-id="69a5f-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="69a5f-104">Če želite pregledati pravilnik, naredite to:</span><span class="sxs-lookup"><span data-stu-id="69a5f-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="69a5f-105">Obiščite središče za [skladnost s predpisi sistema Office & 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)in nato pojdite na pravilnik za **upravljanje groženj** za  >    >  [preprečevanje neželene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="69a5f-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="69a5f-106">Preverite, ali je v **viru pravilnika** prikazano to:  **Add-Xheader/ModifySubject/preusmeritev/brisanje/brez dejanja/SKP**</span><span class="sxs-lookup"><span data-stu-id="69a5f-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="69a5f-107">Če je tako, na zavihku **po meri** preverite nastavitve pravilnika, ki je prizadelo sporočilo.</span><span class="sxs-lookup"><span data-stu-id="69a5f-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="69a5f-108">Možno je, da so **standardne nastavitve** , uporabljene za vse uporabnike storitve Exchange Online, vplivale na sporočilo.</span><span class="sxs-lookup"><span data-stu-id="69a5f-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="69a5f-109">Če želite več informacij o konfiguriranju pravilnikov za filtriranje neželene pošte, glejte [Konfiguracija pravilnikov za filtriranje neželene](https://go.microsoft.com/fwlink/?linkid=2101431)pošte.</span><span class="sxs-lookup"><span data-stu-id="69a5f-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
