---
title: Blokiranje ali deblokiranje zunanjega samodejnega posredovanja e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315890"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokiranje ali deblokiranje samodejnega posredovanja e-pošte

Če želite omogočiti ali onemogočiti posredovanje e-pošte za določen nabiralnik, glejte [Konfiguracija posredovanja e-pošte.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Skrbniki lahko nadzirajo zunanje posredovanje za organizacijo z uporabo pravilnikov [o odhodni neželeni pošti.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Pravilnike za odhodno pošto upravljate na portalu Microsoft 365 Defender na ali z ukazom <https://security.microsoft.com/antispam> »cmdlet« [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) v Exchange Online PowerShell.

Če se prikaže ta napaka: **»550 5.7.520 Access denied, Your organization does not allow external forwarding« (550 5.7.520:** Dostop zavrnjen, vaša organizacija ne dovoli zunanjega posredovanja), preverite, ali je pravilnik konfiguriran tako, da omogoča zunanja samodejno posredovana sporočila.

**Opomba:** Priporočamo privzeto  vrednost Samodejno –  nadzor sistema za nastavitev pravil samodejnega posredovanja v privzetem pravilniku filtriranja odhodne neželene pošte (samodejno zunanje posredovanje je blokirano; notranje samodejno posredovanje še vedno deluje). Ustvarite pravilnike filtriranja odhodne neželene pošte po meri in uporabite vrednost Vklop **–** posredovanje je omogočeno le za uporabnike, ki potrebujejo zunanje samodejno posredovanje e-pošte. Če želite več informacij, glejte [Konfiguriranje zunanjega posredovanja e-pošte v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
