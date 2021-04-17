---
title: Spreminjanje nastavitev omejevanja storitve EWS
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818052"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="9f0eb-102">Spreminjanje nastavitev omejevanja storitve EWS</span><span class="sxs-lookup"><span data-stu-id="9f0eb-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="9f0eb-103">Zaženite naš avtomatiziran preizkus, s katerim lahko spremenite pravilnik omejevanja storitve EWS za trajanje vaše selitve.</span><span class="sxs-lookup"><span data-stu-id="9f0eb-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="9f0eb-104">Upoštevajte, da bodo uvozi storitve EWS tudi po zagonu tega preizkusa še vedno omejeni na 150 MB na 5 minut na nabiralnik. Zaželite višje hitrosti prepustnosti med selitvijo preselite več uporabnikov hkrati.</span><span class="sxs-lookup"><span data-stu-id="9f0eb-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="9f0eb-105">Upoštevajte, da spremembe pravilnika o omejevanju storitve EWS ne vplivajo na te vrste selitve (z Microsoftovimi orodji): hibridno, selitev na mah/selitev po stopnjah (RPC/HTTP), IMAP, G Suite, javna mapa ali storitev PST Import Service.</span><span class="sxs-lookup"><span data-stu-id="9f0eb-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>