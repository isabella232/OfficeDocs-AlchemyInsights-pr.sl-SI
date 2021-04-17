---
title: Ustvarjanje e-poštnega sporočila »Zasuti vse«
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816216"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="b443e-102">Ustvarjanje e-poštnega sporočila »Zasuti vse«</span><span class="sxs-lookup"><span data-stu-id="b443e-102">Create an email catch all</span></span>

<span data-ttu-id="b443e-103">Uporaba catch all is strongly discouraged.</span><span class="sxs-lookup"><span data-stu-id="b443e-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="b443e-104">Pošiljatelju raje pošljite sporočilo o tem, da sporočila ni bilo mogoče dostaviti kot obravnavano, zato da lahko ukrepajo.</span><span class="sxs-lookup"><span data-stu-id="b443e-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="b443e-105">Nadzorujete lahko tudi nabiralnik, ki ste ga spremljali, in tako omejite, da v preteklosti velja le za veljavne e-poštne naslove.</span><span class="sxs-lookup"><span data-stu-id="b443e-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="b443e-106">Vsaka zaseda vse nabiralnike prejme veliko neželene pošte in bo sčasoma lahko zapolnila, če ne bo skrbno nadzorovana.</span><span class="sxs-lookup"><span data-stu-id="b443e-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="b443e-107">(Omejitve prejemanja.)</span><span class="sxs-lookup"><span data-stu-id="b443e-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="b443e-108">Če želite nadaljevati, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="b443e-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="b443e-109">Ustvarite dinamično skupino prejemnikov, & »All Recipient Types« (Vse vrste prejemnikov).</span><span class="sxs-lookup"><span data-stu-id="b443e-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="b443e-110">Ustvarite namenski nabiralnik, da zasukate e-poštna sporočila, na primer catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="b443e-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="b443e-111">Za določeno domeno nastavite DomainType na »InternalRelay«.</span><span class="sxs-lookup"><span data-stu-id="b443e-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="b443e-112">Če pozneje odstranite catch all (zajemi), ne glede na to, ali ste domeno nastavili nazaj na Avtoritativno.</span><span class="sxs-lookup"><span data-stu-id="b443e-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="b443e-113">Prenosno pravilo za poštni tok ustvarite tako:</span><span class="sxs-lookup"><span data-stu-id="b443e-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="b443e-114">Če je pošiljatelj »Zunaj organizacije«</span><span class="sxs-lookup"><span data-stu-id="b443e-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="b443e-115">Preusmeri sporočilo v Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="b443e-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="b443e-116">Razen če je prejemnik član skupine allusers@domain.com (skupina prejemnikov vsebuje vse člane)</span><span class="sxs-lookup"><span data-stu-id="b443e-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="b443e-117">Preverite, ali so novi nabiralniki dodani v dinamično skupino prejemnikov</span><span class="sxs-lookup"><span data-stu-id="b443e-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
