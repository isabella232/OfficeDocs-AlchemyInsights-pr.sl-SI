---
title: Ni mogoče pošiljati/prejemati e-pošte v/iz sistema Office 365 zaradi invalidnosti TLS 1,0 in TLS 1,1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747116"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="3bbb4-102">Ni mogoče pošiljati/prejemati e-pošte v/iz sistema Office 365 zaradi invalidnosti TLS 1,0 in TLS 1,1</span><span class="sxs-lookup"><span data-stu-id="3bbb4-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="3bbb4-103">Kot je potrjeno v središču za sporočila v storitvi MC229914, je TLS 1,0 in TLS 1,1 zastaranje začelo uveljaviti končne točke pretoka pošte za Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="3bbb4-104">Kmalu Office 365 ne bo več sprejel TLS 1,0 in TLS 1,1 e-poštnih povezav iz zunanjih virov.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="3bbb4-105">V storitvi Exchange Online ne boste nikoli uporabili TLS 1,0 ali 1,1 za pošiljanje odhodne e-pošte.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="3bbb4-106">Če se soočate z vprašanji zaradi invalidnosti TLS 1,0 ali 1,1, boste morda doživeli eno od teh napak:</span><span class="sxs-lookup"><span data-stu-id="3bbb4-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="3bbb4-107">Pošiljatelj je dobil poročilo o dokončanju 421 NDR</span><span class="sxs-lookup"><span data-stu-id="3bbb4-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="3bbb4-108">Napaka v pregledovalniku čakalne vrste v strežniku na mestu uporabe, ki pošilja e-pošto uradniku 365 – povezava» 421 4.4.2 je padla zaradi SocketError «</span><span class="sxs-lookup"><span data-stu-id="3bbb4-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="3bbb4-109">Napaka v [dnevniku pošiljanja protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) » Pošlji povezovalnik «na strežniku za pošiljanje e-pošte v Office 365 – pogajanje TLS ni uspelo z napako SocketError</span><span class="sxs-lookup"><span data-stu-id="3bbb4-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="3bbb4-110">Napaka pri pošiljanju ali prejemanju dnevnika protokola Connector –» 451 5.7.3 mora najprej izdati ukaz STARTTLS «</span><span class="sxs-lookup"><span data-stu-id="3bbb4-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="3bbb4-111">Če imate katero koli od zgornjih napak, se prepričajte, da je strežnik, ki pošilja ali prejema e-pošto, omogočen TLS 1,2 s preverjanjem teh registrskih ključev –</span><span class="sxs-lookup"><span data-stu-id="3bbb4-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="3bbb4-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Client] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="3bbb4-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="3bbb4-113">Če spremenite zgornje registrske ključe, da omogočite TLS 1,2, znova zaženite strežnik, da spremembe začnejo veljati.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="3bbb4-114">Preverite tudi, ali imate nameščene najnovejše posodobitve za Windows in Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="3bbb4-115">Za več informacij glejte:</span><span class="sxs-lookup"><span data-stu-id="3bbb4-115">For more information, see:</span></span>

- [<span data-ttu-id="3bbb4-116">Navodila za Exchange Server TLS, del 1: priprava za TLS 1,2 – Skupnost Microsoft tech</span><span class="sxs-lookup"><span data-stu-id="3bbb4-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="3bbb4-117">Microsoft Exchange Server TLS usmerjevalni del 2: Omogočanje TLS 1,2 in prepoznavanje odjemalcev, ki jih ne uporabljajo – skupnost Microsoftove tehnologije</span><span class="sxs-lookup"><span data-stu-id="3bbb4-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="3bbb4-118">Razumevanje scenarijev e-pošte, če različic TLS ni mogoče dogovoriti s storitvijo Exchange Online – skupnost Microsoft tech</span><span class="sxs-lookup"><span data-stu-id="3bbb4-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
