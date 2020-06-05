---
title: Težave pri vpisu v Microsoft 365 apps
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579917"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazen vpisni zaslon v aplikacijah Microsoft 365

Če želite odpraviti to težavo, poskusite naslednje:
- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Ponastavi možnosti Internet Explorerja: pojdite na **Orodja**  >  **Internetne možnosti**  >  **Napredno**  >  **ponastavitev nastavitev Internet Explorerja** (upoštevajte, da boste izgubili nastavitve po meri) in se nato znova poskusite prijaviti v Office.
- Onesposobiti okno zagovornik uporaba zaščita (WDAG) ali poljuben sličen močno žganje ali smešen-kačji strup disciplinski nadzornik v Oxfordu ali Cambridgeu:
    1. Na nadzorni plošči pojdite v **programe**in izberite **Vklopi ali izklopi funkcije sistema Windows**.
    2. Če je Windows Defender Application Guard omogočen, ga poskusite onemogočiti.<br/>
    **Opomba:** Morda boste morali znova zagnati računalnik.
- Zavarovati to mikroskop. AAD. Brokerčep [AAD WAM čep-v](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) je ne bitje tnalo z poljuben uporaba ali močno žganje/smešen-kačji strup disciplinski nadzornik v Oxfordu ali Cambridgeu.
- [Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.<br/>
    **Opomba:** Registrske poti za Office 2016 so se spremenile v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi v Office 2016 graditi 16.0.7967 v operacijskem sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).