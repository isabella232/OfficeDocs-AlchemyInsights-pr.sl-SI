---
title: Ustvarite e-poštni ulov vse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286307"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="f4be9-102">Ustvarite e-poštni ulov vse</span><span class="sxs-lookup"><span data-stu-id="f4be9-102">Create an email catch all</span></span>

<span data-ttu-id="f4be9-103">Uporaba ulova je vse močno odvrnilo.</span><span class="sxs-lookup"><span data-stu-id="f4be9-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="f4be9-104">Bolje je, da zagotovi Odklonijo nazaj pošiljatelju dajanje v najem pošiljatelji vedo svoje sporočilo ni bilo mogoče dostaviti, kot je naslovljena, tako da lahko ukrepajo.</span><span class="sxs-lookup"><span data-stu-id="f4be9-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="f4be9-105">Nadzornem nabiralniku lahko omejite tudi na samo ulov prej veljavnih e-poštnih naslovov.</span><span class="sxs-lookup"><span data-stu-id="f4be9-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="f4be9-106">Vsak ulov vse nabiralnik bo prejel veliko spam in lahko sčasoma izpolnite, če ne pozorno spremljati.</span><span class="sxs-lookup"><span data-stu-id="f4be9-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="f4be9-107">(Obstajajo omejitve, ki prejemajo.)</span><span class="sxs-lookup"><span data-stu-id="f4be9-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="f4be9-108">Če se odločite za nadaljevanje, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="f4be9-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="f4be9-109">Ustvarite dinamično distribucijsko skupino & vključujejo» vse vrste prejemnikov «.</span><span class="sxs-lookup"><span data-stu-id="f4be9-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="f4be9-110">Ustvarite namenski nabiralnik za ulov e-poštnih sporočil, na primer catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="f4be9-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="f4be9-111">Za določeno domeno nastavite DomainType na "Internrelay".</span><span class="sxs-lookup"><span data-stu-id="f4be9-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="f4be9-112">Če vi slej premestitev zgrabiti vsi, obstati varen v število enakih oseb področje prislon v verodostojni.</span><span class="sxs-lookup"><span data-stu-id="f4be9-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="f4be9-113">Ustvarite pravilo za prenos poštnega toka na naslednji način:</span><span class="sxs-lookup"><span data-stu-id="f4be9-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="f4be9-114">Če je pošiljatelj "zunaj organizacije"</span><span class="sxs-lookup"><span data-stu-id="f4be9-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="f4be9-115">Preusmeri sporočilo na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="f4be9-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="f4be9-116">Razen če je prejemnik član allusers@domain.com (distribucijska skupina vsebuje vse člane)</span><span class="sxs-lookup"><span data-stu-id="f4be9-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="f4be9-117">Preverite, ali so novi nabiralniki dodani v dinamično distribucijsko skupino</span><span class="sxs-lookup"><span data-stu-id="f4be9-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
