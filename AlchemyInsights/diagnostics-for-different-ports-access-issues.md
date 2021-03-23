---
title: Diagnostika za različne težave z dostopom do vrat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036808"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="f8ca5-102">Diagnostika za različne težave z dostopom do vrat</span><span class="sxs-lookup"><span data-stu-id="f8ca5-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="f8ca5-103">Če želite odpraviti različne težave z dostopom do vrat, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="f8ca5-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="f8ca5-104">Ustavite/odrazdelite navidezni stroj (VM) iz portala, znova zaženite VM in preskusite znova.</span><span class="sxs-lookup"><span data-stu-id="f8ca5-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="f8ca5-105">Preverite nastavitve omrežja VM, da ugotovite, ali imate za blokiranje prometa varnostne skupine omrežja (NSGs).</span><span class="sxs-lookup"><span data-stu-id="f8ca5-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="f8ca5-106">Uporabite lahko tudi orodje za preverjanje [pretoka IP omrežja v omrežju](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , če želite preveriti, ali je NSGs blokiral promet, User-Defined smeri (UDRs) preusmerjanje prometa na mesto na mestu uporabe (» privzeta pot «0.0.0.0/0) ali v omrežno napravo.</span><span class="sxs-lookup"><span data-stu-id="f8ca5-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="f8ca5-107">Če še vedno prihaja do težav, ko poskušate izvesti zgornje korake, navedite ime VM in vrata TCP, ki jim želite poslati e-pošto za nadaljnjo diagnozo.</span><span class="sxs-lookup"><span data-stu-id="f8ca5-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="f8ca5-108">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="f8ca5-108">**Recommended Documents**</span></span>

[<span data-ttu-id="f8ca5-109">Omejitve in priporočila za pošiljanje odhodne e-pošte prek vrat 25</span><span class="sxs-lookup"><span data-stu-id="f8ca5-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)