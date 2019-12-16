---
title: S/MIME v programu Outlook na spletu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053241"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje e-poštnih sporočil v programu Outlook

Šifriranje sporočil sistema Office 365 je zgrajeno v programu Microsoft Azure Rights Management (Azure RMS), ki je del programa Azure Information Protection. Če vaša naročnina vključuje upravljanje pravic Azure ali varstvo podatkov Azure, **vam ni treba sprejeti nobenih dejanj za ročno Omogočanje ali aktiviranje** storitve za upravljanje pravic.

Na podlagi povratnih informacij strank ne bomo več omogočali pravil o pretoku pošte Exchange za samodejno šifriranje odhodne e-pošte, ki vsebuje določene vrste občutljivih podatkov v vašem najemniku privzeto. Namesto tega ponujamo podrobna navodila o tem, kako lahko to storite sami. Če želite več podrobnosti o ustvarjanju pravila transporta za šifriranje občutljivih informacij, si oglejte [Ta članek](https://aka.ms/OmeEtr).

- Če uporabljate Outlook v spletu (prej **OWA**): ko sestavljate e-poštno sporočilo, preprosto kliknite **zaščitite** v owa. To bo veljalo za dovoljenje» ne Posreduj «. Kliknite **Spremeni dovoljenje** in izberite **šifriranje** , da šifrirate samo sporočilo.

- Če uporabljate **Outlook Client**: Če želite poslati šifrirano sporočilo iz Outlooka 2013 ali 2016 ali Outlook 2016 za Mac, izberite **možnosti** > **dovoljenja**, nato pa izberite možnost zaščite, ki jo potrebujete.

- Če želite **samodejno šifrirati vso e-poštno sporočilo** , poslano nekaterim prejemnikom ali zunanjim partnerskim organizacijam, morate v skrbniškem središču za Exchange ustvariti pravilo za prenos pošte. Podrobna navodila so na voljo v [tem članku za podporo](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

