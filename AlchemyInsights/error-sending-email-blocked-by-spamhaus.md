---
title: Napaka pri pošiljanju e-pošte, ki jo blokira SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813740"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="8f6ae-102">Napaka pri pošiljanju e-pošte: Spamhaus blokira odjemalca gostitelja</span><span class="sxs-lookup"><span data-stu-id="8f6ae-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="8f6ae-103">Naslov IP, s katerega je bilo poslano sporočilo, je na seznamu blokiranih naslovov, ki je v [lasti podjetja Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="8f6ae-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="8f6ae-104">Med razloge za blokiranje s strani podjetja Spamhaus spadajo ogroženi računi, ogroženi računalniki, ki delijo javni naslov IP, in pravilniki ponudnikov internetnih storitev (ISP).</span><span class="sxs-lookup"><span data-stu-id="8f6ae-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="8f6ae-105">Možne popravke so:</span><span class="sxs-lookup"><span data-stu-id="8f6ae-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="8f6ae-106">Za blokirana dohodna sporočila, kjer nadzirate izvorni e-poštni strežnik, morate določiti vzrok in odstraniti blokado s spletnega mesta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="8f6ae-107">Za blokirana dohodna sporočila, kjer naslov IP pripada nekomu drugemu, mora lastnik naslova odstraniti blokado s spletnega mesta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="8f6ae-108">Če je naslov IP na seznamu blokiranih pravilnikov (PBL), lahko lastnik dodeli drugačen statični naslov IP ali odstrani naslov s seznama PBL.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="8f6ae-109">Za blokirana odhodna sporočila iz vaše domene, povezane z Microsoftom, lahko to sporočilo o napaki prejmete, če so sporočila usmerjanje prek storitve drugega ponudnika.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="8f6ae-110">Z orodjem za iskanje WHOIS lahko najdete lastnika blokiranega naslova IP.</span><span class="sxs-lookup"><span data-stu-id="8f6ae-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
