---
title: Preverjanje, ali so v nabiralnikih naslovi za posredovanje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403327"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="b32a4-102">Preverjanje, ali so v nabiralnikih naslovi za posredovanje</span><span class="sxs-lookup"><span data-stu-id="b32a4-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="b32a4-103">Včasih hekerji posredujejo uporabnikova e-poštna sporočila sebi, zato bomo najprej preverili, ali so naslovi in pravila za nabiralnik posredovani.</span><span class="sxs-lookup"><span data-stu-id="b32a4-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="b32a4-104">Nato bomo preverili dnevnike nadzora.</span><span class="sxs-lookup"><span data-stu-id="b32a4-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="b32a4-105">Naslove za posredovanje preverite tako:</span><span class="sxs-lookup"><span data-stu-id="b32a4-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="b32a4-106">Izberite   >  **Uporabniki, ki so aktivni uporabniki.**</span><span class="sxs-lookup"><span data-stu-id="b32a4-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="b32a4-107">Izberite uporabnika, za katerega je bil račun ogrožen.</span><span class="sxs-lookup"><span data-stu-id="b32a4-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="b32a4-108">V prikazanem oknu razširite **Nastavitve pošte** in nato kliknite Uredi za posredovanje  **e-pošte.**</span><span class="sxs-lookup"><span data-stu-id="b32a4-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="b32a4-109">Odstranite vse naslove za posredovanje, ki jih ne prepoznate.</span><span class="sxs-lookup"><span data-stu-id="b32a4-109">Remove any forwarding addresses you don't recognize.</span></span>