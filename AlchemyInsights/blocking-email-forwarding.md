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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478342"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ali odblokiranje posredovanja e-pošte

Če želite omogočiti ali onemogočiti posredovanje e-pošte za določen nabiralnik, glejte [Konfiguracija posredovanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na ravni najemnika se nadzor zunanjega posredovanja izvaja s pravilnikom odhodne neželene pošte. Pravilnik za filtriranje neželene pošte lahko preverite [v središču za](https://protection.office.com/antispam) varnost in skladnost s predpisi ali pa uporabite [ukaz» Get-HostedOutboundSpamFilterPolicy «](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Če se prikaže to sporočilo o napaki: **» 550 5.7.520 Access je zavrnjen, vaša organizacija ne dovoli zunanje posredovanosti «**, preverite, ali je pravilnik konfiguriran tako, da omogoča zunanjo samodejno posredovanje.

**Opomba:** Priporočljivo je, da zunanje samodejno posredovanje onemogočite na privzeti pravilnik za filtriranje neželene pošte in ga omogočite le za uporabnike, ki potrebujejo zunanjo preusmeritev, tako da ustvarijo pravilnik po meri za te uporabnike. Več informacij najdete v članku [Konfiguriranje posredovanja zunanjih e-poštnih sporočil v sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).