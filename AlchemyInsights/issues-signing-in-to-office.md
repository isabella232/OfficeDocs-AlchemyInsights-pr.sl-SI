---
title: Težave pri vpisu v Microsoft 365 aplikacije
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088052"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazen zaslon za vpis v Microsoft 365 aplikacijah

Če želite odpraviti to težavo, poskusite to:
- Namestite najnovejše posodobitve [za](https://support.microsoft.com/help/4027667/windows-10-update) Windows [in Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Ponastavitev možnosti v Internet Explorerju: Pojdite na Orodja za internetne možnosti Napredna ponastavitev programa  >    >    >  **Internet Explorer Nastavitve** (izgubili boste nastavitve po meri) in se nato poskusite znova v Office vpis.
- Onemogočite Windows Defender Application Guard (WDAG) ali podoben požarni zid ali protivirusni program:
    1. Na nadzorni plošči izberite **Programi in** nato izberite Vklop ali **Windows funkcije**.
    2. Če Windows Defender Application Guard je omogočen, ga poskusite onemogočiti.<br/>
    **Opomba:** Morda boste morali znova zagnati računalnik.
- Prepričajte se, da nobenega programa ali požarnega zidu/protivirusnega programa ne blokira vtičnika Microsoft.AAD.Plugin [AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Počistite Office poverilnic](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) s Windows upravitelja poverilnic.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Če želite več informacij, glejte Težave pri vpisu s povezavo po posodobitvi na grad Office [2016 16.0.7967 v Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)