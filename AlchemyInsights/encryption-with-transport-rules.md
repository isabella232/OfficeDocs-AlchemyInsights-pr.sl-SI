---
title: Šifriranje s pravili prenosa
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813884"
---
# <a name="encryption-with-transport-rules"></a>Šifriranje s pravili prenosa

V [skrbniškem središču za Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) lahko uporabite zmogljivosti šifriranja sporočil v Officeu (OME) v pravilih o toku pošte za proženje šifriranja sporočil. V pogoju pravila prenosa izberite možnost **Uporabite šifriranje sporočil v storitvi Office 365 in zaščito pravic**.

- Več informacij najdete v razdelku [Določite pravilo toka pošte za šifriranje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- V storitvi Powershell uporabite pripomoček »cmdlet« [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) in vrednost parametra *ApplyOME* nastavite na $true.
