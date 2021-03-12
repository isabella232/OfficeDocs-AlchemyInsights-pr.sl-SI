---
title: Nabor replik
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714584"
---
# <a name="replica-set"></a><span data-ttu-id="5e89c-102">Nabor replik</span><span class="sxs-lookup"><span data-stu-id="5e89c-102">Replica set</span></span>

<span data-ttu-id="5e89c-103">AADDS je imenovan tudi kot upravljana domena.</span><span class="sxs-lookup"><span data-stu-id="5e89c-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="5e89c-104">To je pravzaprav dva krmilnika domene, ki jih izvaja in vzdržuje backend.</span><span class="sxs-lookup"><span data-stu-id="5e89c-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="5e89c-105">Dva DCs vključujeta en glavni DC in en replikacijski DC.</span><span class="sxs-lookup"><span data-stu-id="5e89c-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="5e89c-106">Varnostne kopije v AADDS (upravljana domena) so avtomatiziran proces, ki ga upravlja Azure platform.</span><span class="sxs-lookup"><span data-stu-id="5e89c-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="5e89c-107">V primeru težave z upravljano domeno vam lahko podpora Azure pomaga pri obnavljanju iz varnostnega kopiranja.</span><span class="sxs-lookup"><span data-stu-id="5e89c-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="5e89c-108">Vsak nabor replik ustvarite v navideznem omrežju.</span><span class="sxs-lookup"><span data-stu-id="5e89c-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="5e89c-109">Vsako navidezno omrežje je treba pokukati v vsako drugo navidezno omrežje, ki gosti nabor replik v upravljani domeni.</span><span class="sxs-lookup"><span data-stu-id="5e89c-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="5e89c-110">S to konfiguracijo ustvarite topologijo omrežja mesh, ki podpira replikacijo imenika.</span><span class="sxs-lookup"><span data-stu-id="5e89c-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="5e89c-111">Navidezno omrežje lahko podpira več naborov replik, pod pogojem, da je vsak nabor replik v drugem navideznem podomrežju.</span><span class="sxs-lookup"><span data-stu-id="5e89c-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="5e89c-112">Če želite več podrobnosti o naboru replik, glejte [nabori pojmov replika](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="5e89c-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
