---
title: 726 Blokiranje posredovanja e-pošte
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059648"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ali deblokiranje posredovanja e-pošte

Če želite omogočiti ali onemogočiti posredovanje e-pošte za določen nabiralnik, glejte [Konfiguracija posredovanja e-pošte.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Na ravni najemnika se nadzor zunanjega posredovanja opravi s pravilnikom o odhodni neželeni pošti. Tukaj ali z ukazom [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)lahko preverite pravilnik filtriranja odhodne neželene pošte v središču za varnost in skladnost s predpisi. [](https://protection.office.com/antispam)

Če se prikaže to sporočilo o napaki: **»550 5.7.520** Dostop je zavrnjen, vaša organizacija ne dovoli zunanjega posredovanja«, preverite, ali je pravilnik konfiguriran tako, da omogoča zunanje samodejno posredovanje.

**Opomba:** Priporočljivo je, da je zunanji samodejni skrbnik onemogočen za privzeti pravilnik filtriranja odhodne pošte in ga omogočite le za uporabnike, ki potrebujejo zunanje posredovanje, tako da tem uporabnikom ustvarite pravilnik po meri. Več o tem lahko preberete [v možnosti Konfiguracija zunanjega posredovanja e-Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)