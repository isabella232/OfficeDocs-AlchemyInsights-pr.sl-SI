---
title: 2681 Attack simulator v uradu 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305347"
---
# <a name="attack-simulator-in-office-365"></a>Attack simulator v uradu 365

- Ali ste manjka Attack simulator? Attack simulator zahteva **office 365 napredno zaščito pred grožnjami načrt 2 (ATP načrt 2)** ali **Office 365 Enterprise E5**. Attack simulator ni **vključen v** Office 365 napredno zaščito pred grožnjami načrt 1 (ATP načrt 1), Office 365 Enterprise E3, ali kateri koli Office 365 poslovne naročnine.

- Račun, ki ga uporabljate za zagon simuliranih napadov, zahteva globalne skrbniške ali varnostne skrbniške pravice in večfaktorsko preverjanje pristnosti (MFA). Če želite več informacij o zahtevah za Attack simulator, si oglejte [to temo](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Važen stvari znati približno **živalski moč parola** napad Simulations:

  - Če je ciljni račun omogočen MFA in je bilo geslo pravilno ugano, račun ne bo prikazan kot ogrožen (drugi faktor za preverjanje pristnosti bo nepopoln).

  - Datoteka z geslom ne more biti večja od 10 MB. Uporabite eno geslo na vrstico in na seznamu vključite prazno črto (povratni prevoz).

- Pomembne stvari vedeti o **kopje phishing** priložite simulacije:

  - Po zasnovi ne morete zagotoviti vrednosti po meri za **URL strežnika za prijavo lažnega predstavljanja**.

  - Če prejemnik uporabi možnost [Omogoči dodajanje sporočila poročila](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , da sporočilo sporoči kot lažno predstavljanje, morda ne boste prejeli opozoril za sporočilo (ker je to simuliran napad).

- Poročila: ko je simuliran napad končan, lahko kliknete **napad podrobnosti** , da si ogledate poročilo.

- Za podrobna navodila in nove funkcije v Attack simulator, glej [Attack simulator v uradu 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
