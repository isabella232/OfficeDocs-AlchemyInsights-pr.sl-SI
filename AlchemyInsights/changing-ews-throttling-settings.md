---
title: Spreminjanje nastavitev omejevanja storitve EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075913"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="6eca8-102">Spreminjanje nastavitev omejevanja storitve EWS</span><span class="sxs-lookup"><span data-stu-id="6eca8-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="6eca8-103">Zaženite naš avtomatiziran preizkus, s katerim lahko spremenite pravilnik omejevanja storitve EWS za trajanje vaše selitve.</span><span class="sxs-lookup"><span data-stu-id="6eca8-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="6eca8-104">Upoštevajte, da bodo uvozi storitve EWS tudi po zagonu tega preizkusa še vedno omejeni na 150 MB na 5 minut na nabiralnik. Zaželite višje hitrosti prepustnosti med selitvijo preselite več uporabnikov hkrati.</span><span class="sxs-lookup"><span data-stu-id="6eca8-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="6eca8-105">Upoštevajte, da spremembe pravilnika o omejevanju storitve EWS ne vplivajo na te vrste selitve (z Microsoftovimi orodji): hibridno, selitev na mah/selitev po stopnjah (RPC/HTTP), IMAP, G Suite, javna mapa ali storitev PST Import Service.</span><span class="sxs-lookup"><span data-stu-id="6eca8-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>