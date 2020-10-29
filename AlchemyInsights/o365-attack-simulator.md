---
title: 2681 simulator napada v Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801567"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulator napada v programu Microsoft 365

- Ali zamujate simulator napada? Simulator napada zahteva **Microsoft Defender za office 365 (paket ATP 2)** ali **Office 365 Enterprise E5** . Simulator napada ni **vključen v** Microsoft Defender za Office 365 (paket ATP 1), Office 365 Enterprise E3 ali kateri koli Microsoft 365 apps za naročnine na podjetja.

- Z računom, ki ga uporabljate za zagon simuliranih napadov, potrebujete dovoljenja globalnega skrbnika ali varnostnega skrbnika in multi-Factor Authentication (MFA). Če želite več informacij o zahtevah simulatorja napada, si oglejte [to temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Pomembne stvari, ki jih morate vedeti o simulacijah **nasilnih napadov gesel** :

  - Če je v ciljnem računu omogočena funkcija MFA in je bilo geslo pravilno uganil, račun ne bo prikazan kot ogrožen (drugi faktor preverjanja pristnosti bo nepopoln).

  - Datoteka gesel ne more biti večja od 10 MB. Uporabite eno geslo na vrstico in vključite prazno vrstico (vračanje) po zadnjem geslu na seznamu.

- Pomembne stvari, ki jih morate vedeti o prilaganju simulacij s **kopjem** :

  - Po načrtu ne morete ponuditi vrednosti po meri za **spletni naslov strežnika za prijavo lažnega predstavljanja** .

  - Če prejemnik uporabi [dodatek» omogoči sporočilo za poročilo](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) «, da sporoči sporočilo kot lažno predstavljanje, morda ne boste prejeli opozoril za sporočilo (ker je to simulirani napad).

- Poročila: ko je simulirani napad končan, lahko kliknete **podrobnosti napada** , da si ogledate poročilo.

- Če želite podrobna navodila in nove funkcije v simulatorju napada, glejte [simulator napada v programu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
