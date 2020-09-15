---
title: Težave pri vpisu v programe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695303"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazen zaslon za vpis v aplikacijah Microsoft 365

Če želite odpraviti to težavo, naredite to:
- Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Ponastavitev možnosti Internet Explorerja: pojdite v razdelek **Orodja**  >  **Internetne možnosti**  >  **Napredno**  >  **ponastavitev nastavitev Internet Explorerja** (upoštevajte, da boste izgubili nastavitve po meri), nato pa se poskusite znova vpisati v Office.
- Onemogočite aplikacijo Guard (WDAG) programa Windows Defender ali kateri koli podoben požarni zid ali protivirusni program:
    1. Na nadzorni plošči pojdite v razdelek **programi**in nato izberite **Vklopi ali izklopi funkcije sistema Windows**.
    2. Če je omogočena zaščita programa Windows Defender, jo poskusite onemogočiti.<br/>
    **Opomba:** Morda boste morali znova zagnati računalnik.
- Zagotovite, da [vtičnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. zvočna WAM. BrokerPlugin ne blokira noben program ali požarni zid/protivirusni program.
- [Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.<br/>
    **Opomba:** Poti registra za Office 2016 so se spremenile v 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi na Office 2016 Build 16.0.7967 v sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).