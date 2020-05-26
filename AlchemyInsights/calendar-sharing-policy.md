---
title: 618 koledar črepina zvitost
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373015"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="cff87-102">Napaka pravilnika pri skupni rabi koledarja</span><span class="sxs-lookup"><span data-stu-id="cff87-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="cff87-103">Naredite nekaj od tega, kot je primerno za vaše stanje:</span><span class="sxs-lookup"><span data-stu-id="cff87-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="cff87-104">Vzpostavite povezavo s storitvijo Exchange Online z oddaljenim PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cff87-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="cff87-105">Če želite več informacij, glejte [Vzpostavljanje povezave s storitvijo Exchange Online z oddaljenim PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="cff87-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="cff87-106">V krajevnem strežniku odprite lupino za upravljanje Exchangeevega.</span><span class="sxs-lookup"><span data-stu-id="cff87-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="cff87-107">Določite pravilnik o delitvi, ki je dodeljen uporabniku.</span><span class="sxs-lookup"><span data-stu-id="cff87-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="cff87-108">Če želite to narediti, zaženite ta ukaz in upoštevajte, da se je pravilnik vrnil:</span><span class="sxs-lookup"><span data-stu-id="cff87-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="cff87-109">Posodobite pravilnik o skupni rabi za uporabnika.</span><span class="sxs-lookup"><span data-stu-id="cff87-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="cff87-110">Če želite to narediti, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="cff87-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="cff87-111">Odprite skrbniški center Exchange.</span><span class="sxs-lookup"><span data-stu-id="cff87-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="cff87-112">Kliknite **organizacija**in nato dvokliknite pravilnik, ki je dodeljen uporabniku v okviru **posamezne skupne rabe**.</span><span class="sxs-lookup"><span data-stu-id="cff87-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="cff87-113">To je pravilnik, ki je bil vrnjen v koraku 2.</span><span class="sxs-lookup"><span data-stu-id="cff87-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="cff87-114">Na strani pravilo delitve izberite raven skupne rabe koledarja, ki jo želite dovoliti v razdelku **določanje, katere informacije želite deliti z drugimi**; kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="cff87-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="cff87-115">Če želite več informacij, glejte: [» pravilnik ne dovoljuje dodelitve dovoljenj na tej ravni enemu ali več napaki prejemnika «, ko uporabnik poskuša deliti koledar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="cff87-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
