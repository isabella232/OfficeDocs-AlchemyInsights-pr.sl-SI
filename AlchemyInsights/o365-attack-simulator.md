---
title: 2681 Attack simulator v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506754"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack simulator v Microsoft 365

- Ali ste manjka Attack simulator? Attack simulator zahteva **office 365 napredno zaščito pred grožnjami načrt 2 (ATP načrt 2)** ali **Office 365 Enterprise E5**. Attack simulator ni **vključen v** Office 365 napredno zaščito pred grožnjami načrt 1 (ATP plan 1), Office 365 Enterprise E3, ali katere koli Microsoftove 365 apps za poslovne naročnine.

- Račun, ki ga uporabljate za zagon simuliranih napadov, zahteva globalne skrbniške ali varnostne skrbniške pravice in večfaktorsko preverjanje pristnosti (MFA). Če želite več informacij o zahtevah za Attack simulator, si oglejte [to temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Važen stvari znati približno **živalski moč parola** napad Simulations:

  - Če je ciljni račun omogočen MFA in je bilo geslo pravilno ugano, račun ne bo prikazan kot ogrožen (drugi faktor za preverjanje pristnosti bo nepopoln).

  - Datoteka z geslom ne more biti večja od 10 MB. Uporabite eno geslo na vrstico in na seznamu vključite prazno črto (povratni prevoz).

- Pomembne stvari vedeti o **kopje phishing** priložite simulacije:

  - Po zasnovi ne morete zagotoviti vrednosti po meri za **URL strežnika za prijavo lažnega predstavljanja**.

  - Če prejemnik uporabi možnost [Omogoči dodajanje sporočila poročila](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , da sporočilo sporoči kot lažno predstavljanje, morda ne boste prejeli opozoril za sporočilo (ker je to simuliran napad).

- Poročila: ko je simuliran napad končan, lahko kliknete **napad podrobnosti** , da si ogledate poročilo.

- Za podrobna navodila in nove funkcije v Attack simulator, glej [Attack simulator v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
