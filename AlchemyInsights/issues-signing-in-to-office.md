---
title: Težave pri vpisu v aplikacije Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833055"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazen zaslon za vpis v aplikacijah Microsoft 365

Če želite odpraviti to težavo, poskusite to:
- Namestite najnovejše posodobitve za [Windows in](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Ponastavitev možnosti v Internet Explorerju: Pojdite na Orodja za internetne možnosti Napredne nastavitve  >    >    >  **Internet Explorerja** (upoštevajte, da boste izgubili nastavitve po meri) in se nato znova poskusite vstaviti v Office.
- Onemogočite Windows Defender Application Guard (WDAG) ali podoben požarni zid ali protivirusni program:
    1. Na nadzorni plošči izberite **Programi in** nato vklop ali izklop funkcij **sistema Windows.**
    2. Če je windows Defender Application Guard omogočen, ga poskusite onemogočiti.<br/>
    **Opomba:** Morda boste morali znova zagnati računalnik.
- Prepričajte se, da nobenega programa ali požarnega zidu/protivirusnega programa ne blokira vtičnika Microsoft.AAD.Plugin [AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Počistite poverilnice za Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Če želite več informacij, glejte Težave pri vpisu s povezavo po posodobitvi na [gradovi Office 2016, graden 16.0.7967 v sistemu Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)