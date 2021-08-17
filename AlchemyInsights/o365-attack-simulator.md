---
title: 2681 Attack Rio in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895807"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Rio in Microsoft 365

- Ali pogrešate napadajoče napade? Plan 2 ali **Office 365 (paket 2)** ali **paket E5 zahteva Office 365 Enterprise Defender**. Storitev Attack Premium **ni vključena** v Microsoft Defender za Office 365 paket 1, Office 365 Enterprise E3 ali katere koli Programi Microsoft 365 za manjša podjetja naročnine.

- Račun, ki ga uporabljate za zagon simuliranih napadov, zahteva dovoljenja globalnega skrbnika ali skrbnika za varnost in večkratno preverjanje pristnosti (MFA). Če želite več informacij o zahtevah napadov z napadom, si [oglejte to temo.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Pomembne stvari, ki jih je treba vedeti **o simulacijah napadov z** grobih geslih:

  - Če je v ciljnem računu omogočena storitev MFA in je bilo pravilno ugibanje gesla, račun ne bo prikazan kot ogrožen (drugi dejavnik preverjanja pristnosti bo nepopoln).

  - Datoteka z geslom ne sme biti večja od 10 MB. Uporabite eno geslo na vrstico in vključite prazno vrstico (prelom vrstice) za zadnjim geslom na seznamu.

- Pomembne stvari, ki jih je treba vedeti **o simulacijah prilaganja spearnega** lažnega predstavljanja:

  - Privzeto ni mogoče vati vrednosti po meri za URL strežnika za prijavo v lažno **predstavljanje.**

  - Če prejemnik uporablja dodatek Omogoči sporočilo poročila [za](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) poročanje o sporočilu kot lažno predstavljanje, morda ne boste prejeli opozoril za sporočilo (ker gre za simuliran napad).

- Poročila: Ko je simulacija napada končana, lahko kliknete **Podrobnosti** o napadu, da si ogledate poročilo.

- Če želite podrobna navodila in nove funkcije v napadaalni napadu, glejte [Attack Rio v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
