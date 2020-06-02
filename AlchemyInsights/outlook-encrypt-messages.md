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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511524"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje e-poštnih sporočil v programu Outlook

Microsoft 365 sporočilo encryption je zidava naprej mikroskop Azure pravilen uprava (Azure RMS), kateri je del od Azure sporočilo varstvo. Če vaša naročnina vključuje upravljanje pravic Azure ali varstvo podatkov Azure, **vam ni treba sprejeti nobenih dejanj za ročno Omogočanje ali aktiviranje** storitve za upravljanje pravic.

Na podlagi povratnih informacij strank ne bomo več omogočali pravil o pretoku pošte Exchange za samodejno šifriranje odhodne e-pošte, ki vsebuje določene vrste občutljivih podatkov v vašem najemniku privzeto. Namesto tega ponujamo podrobna navodila o tem, kako lahko to storite sami. Če želite več podrobnosti o ustvarjanju pravila transporta za šifriranje občutljivih informacij, si oglejte [Ta članek](https://aka.ms/OmeEtr).

- Če uporabljate Outlook v spletu (prej **OWA**): ko sestavljate e-poštno sporočilo, preprosto kliknite **zaščitite** v owa. To bo veljalo za dovoljenje» ne Posreduj «. Kliknite **Spremeni dovoljenje** in izberite **šifriranje** , da šifrirate samo sporočilo.

- Če uporabljate **Outlookovo stranko**: Če želite poslati šifrirano sporočilo iz Outlooka 2013 ali 2016 ali Outlook 2016 za Mac, izberite **možnosti**  >  **dovoljenja**, nato izberite zaščito, ki jo potrebujete.

- Če želite **samodejno šifrirati vso e-poštno sporočilo** , poslano nekaterim prejemnikom ali zunanjim partnerskim organizacijam, morate v skrbniškem središču za Exchange ustvariti pravilo za prenos pošte. Podrobna navodila so na voljo v [tem članku za podporo](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

