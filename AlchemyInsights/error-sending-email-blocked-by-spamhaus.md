---
title: Napaka pri pošiljanju e-pošte blokirana, ki jih SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714274"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="e5fe0-102">Napaka pri pošiljanju e-pošte: odjemalec gostitelja blokiran z Spamhaus</span><span class="sxs-lookup"><span data-stu-id="e5fe0-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="e5fe0-103">IP naslov, ki je poslal sporočilo, je na blok seznam v lasti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="e5fe0-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="e5fe0-104">Razlogi za blokado s strani Spamhaus vključujejo ogrožene račune, ogrožene stroje, ki delijo javni naslov IP in pravilnike ponudnika internetnih storitev (ISP).</span><span class="sxs-lookup"><span data-stu-id="e5fe0-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="e5fe0-105">Možni popravki so:</span><span class="sxs-lookup"><span data-stu-id="e5fe0-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="e5fe0-106">Za blokirana dohodna sporočila, kjer nadzirate izvorni e-poštni strežnik, morate ugotoviti vzrok in odstraniti blok iz spletne strani Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="e5fe0-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="e5fe0-107">Za blokirana dohodna sporočila, kjer je izvorni IP naslov pripada nekomu drugemu, mora lastnik naslova odstraniti blok iz spletne strani Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="e5fe0-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="e5fe0-108">Če je naslov IP na seznamu blokiranih pravilnikov (PBL), lahko lastnik dodeli drug statični naslov IP ali odstrani naslov iz PBL.</span><span class="sxs-lookup"><span data-stu-id="e5fe0-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="e5fe0-109">Za blokirana odhodna sporočila iz vaše domene, povezane z Microsoftom, lahko to napako prejmete, če so sporočila preusmerjena skozi storitev 3rd Party.</span><span class="sxs-lookup"><span data-stu-id="e5fe0-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="e5fe0-110">Za iskanje blokiranega lastnika naslova IP lahko uporabite orodje za iskanje WHOIS.</span><span class="sxs-lookup"><span data-stu-id="e5fe0-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
