---
title: Zaradi onemogočanja TLS 1.0 in TLS 1.1 Office 365 ni mogoče pošiljati/prejemati e-pošte v/iz storitve
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054922"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Zaradi onemogočanja TLS 1.0 in TLS 1.1 Office 365 ni mogoče pošiljati/prejemati e-pošte v/iz storitve

Kot je potrjeno v objavi središča za sporočila MC229914, so se za končne točke toka pošte začele uveljavljati TLS 1.0 in TLS 1. Exchange Online 1. Kmalu Office 365 ne boste več sprejeli e-poštnih povezav TLS 1.0 in TLS 1.1 iz zunanjih virov. Poleg tega Exchange Online nikoli ne bodo uporabljali TLS 1.0 ali 1.1 za pošiljanje odhodne e-pošte. Če imate težave zaradi onemogočanja TLS 1.0 ali 1.1, lahko pride do ene od teh napak–

- Pošiljatelj je zaradi socketError opustil odklon sporočila o neuspeli dostavi – povezava je bila opuščena na »421 4.4.2«.
- Napaka v pregledovalniku čakalne vrste strežnika na mestu uporabe, ki pošilja e-pošto v oficirja 365 – '421 4.4.2 Connection dropped due to SocketError'
- Napaka v dnevniku protokola za pošiljanje [povezovalnika](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) v strežniku, ki pošilja e-pošto v Office 365- TLS pogajanje ni uspelo z napako SocketError
- Napaka v dnevniku protokola protokola za pošiljanje ali prejemanje – '451 5.7.3 Najprej je treba izdati ukaz STARTTLS'

Če pride do katere koli od zgornjih napak, preverite, ali je v strežniku, ki pošilja ali prejema e-pošto, omogočen TLS 1.2, tako da preverite te registrske ključe –

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Če spremenite zgornje registrske ključe, da omogočite TLS 1.2, znova zaženite strežnik, da bodo spremembe začele veljati. Poleg tega se prepričajte, da imate nameščene najnovejše Windows in Exchange posodobitve.

Če želite več informacij, si oglejte:

- [Exchange Server Navodila za TLS, 1. del: Pripravljamo za TLS 1.2 – Microsoftova tehnična skupnost](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server 2. del smernic za TLS: Omogočanje TLS 1.2 in prepoznavanje odjemalcev, ki ga ne uporabljajo – Microsoftova tehnična skupnost](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Razumevanje scenarijev e-pošte, če se o različicah TLS ne morete strinjati s Exchange Online – Microsoftova tehnična skupnost](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
