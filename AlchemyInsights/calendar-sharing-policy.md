---
title: Pravilnik o skupni rabi koledarja 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684246"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="2f28b-102">Napaka pravilnika pri skupni rabi koledarja</span><span class="sxs-lookup"><span data-stu-id="2f28b-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="2f28b-103">Naredite nekaj od tega, odvisno od tega, ali je to primerno za vaše stanje:</span><span class="sxs-lookup"><span data-stu-id="2f28b-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="2f28b-104">Vzpostavljanje povezave s storitvijo Exchange Online z uporabo oddaljenega PowerShella.</span><span class="sxs-lookup"><span data-stu-id="2f28b-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="2f28b-105">Če želite več informacij, glejte [Vzpostavljanje povezave s storitvijo Exchange Online z oddaljeno lupino PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2f28b-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="2f28b-106">V strežniku na mestu uporabe odprite lupino za upravljanje Exchangea.</span><span class="sxs-lookup"><span data-stu-id="2f28b-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="2f28b-107">Določite pravilnik o skupni rabi, ki je dodeljen uporabniku.</span><span class="sxs-lookup"><span data-stu-id="2f28b-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="2f28b-108">Če želite to narediti, zaženite ta ukaz in zapomnite, da je pravilnik vrnjen:</span><span class="sxs-lookup"><span data-stu-id="2f28b-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="2f28b-109">Posodobite pravilnik o skupni rabi za uporabnika.</span><span class="sxs-lookup"><span data-stu-id="2f28b-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="2f28b-110">Če želite to narediti, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="2f28b-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="2f28b-111">Odprite skrbniško središče za Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f28b-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="2f28b-112">Kliknite **organizacija**in nato dvokliknite pravilnik, ki je uporabniku dodeljen v okviru **posamezne skupne rabe**.</span><span class="sxs-lookup"><span data-stu-id="2f28b-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="2f28b-113">To je pravilnik, ki je bil vrnjen v koraku 2.</span><span class="sxs-lookup"><span data-stu-id="2f28b-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="2f28b-114">Na strani pravilo skupne rabe izberite raven skupne rabe koledarja, ki jo želite omogočiti v razdelku **določanje podatkov, ki jih želite dati v skupno rabo**; kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="2f28b-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="2f28b-115">Če želite več informacij, si oglejte: [» pravilnik ne dovoljuje dodeljevanja dovoljenj na tej ravni za enega ali več uporabnikov «napak, ko uporabnik poskuša dati koledar v skupno rabo](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="2f28b-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
