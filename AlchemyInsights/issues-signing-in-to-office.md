---
title: Vprašanja, ki se vpisujete Office aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938343"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Obrazec vpisni zaslon v Office aplikacije

Če želite odpraviti težavo, poskusite naslednje:
- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Ponastavite možnosti Internet Explorerja: iti k **rokodelsko orodje** > **Internetne možnosti** > **Advanced** > **Ponastavljanje nastavitev programa Internet Explorer** (upoštevajte, da boste izgubili nastavitve po meri) in nato poskusite vpisujete Office znova.
- Onesposobiti okno zagovornik uporabe straže (WDAG) ali podoben program močno žganje ali smešen-kačji strup:
    1. V nadzorni plošči, iti k **Programs**, in nato izberite **zavoj okno zunanja oblika naprej ali ne sveže**.
    2. Če je omogočen Windows Defender uporabo straže, poskusite onemogočiti to.<br/>
    **Opomba:** Boste morda morali ponovno zagnati računalnik.
- Zagotoviti, da Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne bo blokirala vsak program ali požarni zid/smešen-kačji strup program.
- [Jasno urad poverilnic](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.<br/>
    **Opomba:** Registrske poti za Office 2016 spremenili v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Če želite več informacij, glejte [te¾ave pri povezovanju v vpisno po posodobitvi za Office 2016 zidava 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).