---
title: 726 blokiranje posredovanja e-pošte
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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219871"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ali odblokiranje posredovanja e-pošte

Če želite omogočiti ali onemogočiti posredovanje e-pošte za določen nabiralnik, glejte [Konfiguracija posredovanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na ravni najemnika se nadzor zunanjega posredovanja izvaja s pravilnikom odhodne neželene pošte. Če je nastavljena na izklopljeno ali samodejno, lahko blokira posredovanje e-pošte s storitvijo» 550 5.7.520 Access je zavrnjena, vaša organizacija ne dovoljuje zunanjega posredovanja «. Če je bila preusmeritev nastavljena na blokirano, je to napaka, ki jo bodo videli uporabniki.

Če je preusmeritev blokirana, se prepričajte, da je pravilnik konfiguriran tako, da omogoča zunanjo samoposredovanje. Pravilnik za filtriranje neželene pošte lahko preverite v središču za varnost in skladnost s predpisi ali z ukazom Get-HostedOutboundSpamFilterPolicy | ime FL, AutoForwardingMode. Če želite nastaviti samodejno blokiranje blokiranja, vam bo isti ukaz povedal trenutno stanje pravilnika.

Opomba: priporočamo, da zunanje samodejno posredovanje onemogočite na privzetem pravilniku za filtriranje neželene pošte in jo omogočite le za uporabnike, ki potrebujejo zunanjo preusmeritev tako, da ustvarijo pravilnik po meri za te uporabnike. Več informacij najdete v članku [Konfiguriranje posredovanja zunanjih e-poštnih sporočil v sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).