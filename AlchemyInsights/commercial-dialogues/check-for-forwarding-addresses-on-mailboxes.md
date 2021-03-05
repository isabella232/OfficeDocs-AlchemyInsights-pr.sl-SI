---
title: Preverjanje naslovov za posredovanje v nabiralnikih
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483924"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="0ea03-102">Preverjanje naslovov za posredovanje v nabiralnikih</span><span class="sxs-lookup"><span data-stu-id="0ea03-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="0ea03-103">Včasih hekerji posredujejo e-poštna sporočila uporabnikov, tako da najprej preverimo, ali so naslovi za posredovanje in pravila v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="0ea03-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="0ea03-104">Nato bomo preverili dnevnike nadzora.</span><span class="sxs-lookup"><span data-stu-id="0ea03-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="0ea03-105">Oglejte si navodila za preverjanje naslovov za posredovanje:</span><span class="sxs-lookup"><span data-stu-id="0ea03-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="0ea03-106">Izberite **Uporabniki**  >  **aktivni uporabniki**.</span><span class="sxs-lookup"><span data-stu-id="0ea03-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="0ea03-107">Izberite uporabnika, katerega račun je bil ogrožen.</span><span class="sxs-lookup"><span data-stu-id="0ea03-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="0ea03-108">V flyout, ki se prikaže, razširite **Nastavitve pošte** in nato kliknite **Uredi** za **posredovanje e-pošte**.</span><span class="sxs-lookup"><span data-stu-id="0ea03-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="0ea03-109">Odstranite vse naslove za posredovanje, ki jih ne prepoznate.</span><span class="sxs-lookup"><span data-stu-id="0ea03-109">Remove any forwarding addresses you don't recognize.</span></span>