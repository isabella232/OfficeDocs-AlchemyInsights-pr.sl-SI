---
title: Ustvarjanje e-poštnega ulova
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713002"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="79f53-102">Ustvarjanje e-poštnega ulova</span><span class="sxs-lookup"><span data-stu-id="79f53-102">Create an email catch all</span></span>

<span data-ttu-id="79f53-103">Uporaba ulova je zelo odvrnjena.</span><span class="sxs-lookup"><span data-stu-id="79f53-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="79f53-104">Bolje je, da pošljete pošiljateljem, da se ne morejo dostaviti tako, da bodo lahko ukrepali, če želite poslati odklon.</span><span class="sxs-lookup"><span data-stu-id="79f53-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="79f53-105">Nadzorovani nabiralnik lahko omejite tudi tako, da ujamete le prej veljavne e-poštne naslove.</span><span class="sxs-lookup"><span data-stu-id="79f53-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="79f53-106">Vsak ulov nabiralnika bo prejel dobro ponudbo neželene pošte in lahko sčasoma zapolni, če ni pozorno spremljati.</span><span class="sxs-lookup"><span data-stu-id="79f53-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="79f53-107">(Obstajajo omejitve za prejemanje.)</span><span class="sxs-lookup"><span data-stu-id="79f53-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="79f53-108">Če se odločite nadaljevati, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="79f53-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="79f53-109">Ustvarjanje dinamične distribucijske skupine & vključuje» vse vrste prejemnikov «.</span><span class="sxs-lookup"><span data-stu-id="79f53-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="79f53-110">Ustvarjanje namenskega nabiralnika za lovljenje e-poštnih sporočil, na primer catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="79f53-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="79f53-111">Za določeno domeno nastavite DomainType na» InternalRelay «.</span><span class="sxs-lookup"><span data-stu-id="79f53-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="79f53-112">Če pozneje odstranite vse, se prepričajte, da je domena nastavljena na avtoritativno.</span><span class="sxs-lookup"><span data-stu-id="79f53-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="79f53-113">Ustvarite pravilo za prenos Mailflow, kot sledi:</span><span class="sxs-lookup"><span data-stu-id="79f53-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="79f53-114">Če je pošiljatelj» zunaj organizacije «</span><span class="sxs-lookup"><span data-stu-id="79f53-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="79f53-115">Preusmeritev sporočila v Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="79f53-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="79f53-116">Razen če je prejemnik član allusers@domain.com (skupina prejemnikov vsebuje vse člane)</span><span class="sxs-lookup"><span data-stu-id="79f53-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="79f53-117">Preverite veljavnost novih nabiralnikov v dinamični distribucijski skupini.</span><span class="sxs-lookup"><span data-stu-id="79f53-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
