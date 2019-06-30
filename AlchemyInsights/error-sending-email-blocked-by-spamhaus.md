---
title: Napaka, pošiljanje e-pošte, ki blokira SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387865"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="30f37-102">Napaka pri pošiljanju e-pošte: odjemalca gostitelja blokiran z Spamhaus</span><span class="sxs-lookup"><span data-stu-id="30f37-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="30f37-103">IP naslov, ki je poslal sporočilo, je na seznamu blokiranih mest v lasti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="30f37-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="30f37-104">Razlogi za blokirala Spamhaus vključujejo ogrožena računov, ogrožena stroji delitev javni IP naslov in ponudnika internetnih storitev (ISP) pravila.</span><span class="sxs-lookup"><span data-stu-id="30f37-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="30f37-105">Možni popravki so:</span><span class="sxs-lookup"><span data-stu-id="30f37-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="30f37-106">Za blokirane dohodna sporočila Office 365, če nadzirate strežnik vir e-pošte, boste morali ugotoviti vzrok in odstrani blokiranja na spletni strani Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="30f37-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="30f37-107">Za blokirane dohodna sporočila Office 365, kjer izvorni IP naslov pripada nekomu drugemu, naslov lastnik mora umakniti blok na spletni strani Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="30f37-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="30f37-108">Če je IP naslov na seznam blok politike (PBL), lastnik lahko dodelite različne statični naslov IP ali naslov odstranite na PBL.</span><span class="sxs-lookup"><span data-stu-id="30f37-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="30f37-109">Za blokirane odhodnih sporočil iz vaše domene Office 365, lahko prejmete to napako, če sporočila so preusmerjeni preko 3rd stranka storitev.</span><span class="sxs-lookup"><span data-stu-id="30f37-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="30f37-110">Uporabite lahko orodje za iskanje WHOIS najti lastnika blokiranih IP naslov.</span><span class="sxs-lookup"><span data-stu-id="30f37-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
