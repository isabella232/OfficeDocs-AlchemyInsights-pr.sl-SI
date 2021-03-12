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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Ni mogoče pošiljati/prejemati e-pošte v/iz sistema Office 365 zaradi invalidnosti TLS 1,0 in TLS 1,1

Kot je potrjeno v središču za sporočila v storitvi MC229914, je TLS 1,0 in TLS 1,1 zastaranje začelo uveljaviti končne točke pretoka pošte za Exchange Online. Kmalu Office 365 ne bo več sprejel TLS 1,0 in TLS 1,1 e-poštnih povezav iz zunanjih virov. V storitvi Exchange Online ne boste nikoli uporabili TLS 1,0 ali 1,1 za pošiljanje odhodne e-pošte. Če se soočate z vprašanji zaradi invalidnosti TLS 1,0 ali 1,1, boste morda doživeli eno od teh napak:

- Pošiljatelj je dobil poročilo o dokončanju 421 NDR
- Napaka v pregledovalniku čakalne vrste v strežniku na mestu uporabe, ki pošilja e-pošto uradniku 365 – povezava» 421 4.4.2 je padla zaradi SocketError «
- Napaka v [dnevniku pošiljanja protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) » Pošlji povezovalnik «na strežniku za pošiljanje e-pošte v Office 365 – pogajanje TLS ni uspelo z napako SocketError
- Napaka pri pošiljanju ali prejemanju dnevnika protokola Connector –» 451 5.7.3 mora najprej izdati ukaz STARTTLS «

Če imate katero koli od zgornjih napak, se prepričajte, da je strežnik, ki pošilja ali prejema e-pošto, omogočen TLS 1,2 s preverjanjem teh registrskih ključev –

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Client] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**

Če spremenite zgornje registrske ključe, da omogočite TLS 1,2, znova zaženite strežnik, da spremembe začnejo veljati. Preverite tudi, ali imate nameščene najnovejše posodobitve za Windows in Exchange.

Za več informacij glejte:

- [Navodila za Exchange Server TLS, del 1: priprava za TLS 1,2 – Skupnost Microsoft tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Microsoft Exchange Server TLS usmerjevalni del 2: Omogočanje TLS 1,2 in prepoznavanje odjemalcev, ki jih ne uporabljajo – skupnost Microsoftove tehnologije](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Razumevanje scenarijev e-pošte, če različic TLS ni mogoče dogovoriti s storitvijo Exchange Online – skupnost Microsoft tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
