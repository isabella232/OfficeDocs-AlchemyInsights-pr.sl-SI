---
title: S/MIME v Outlook v spletu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010740"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje e-poštnih sporočil v Outlook

Microsoft 365 Šifriranje sporočil temelji na storitvi Microsoft Azure Rights Management (Azure RMS), ki je del storitve Azure Information Protection. Če vaša naročnina vključuje Azure Rights Management ali Azure Information **Protection,** vam ni treba narediti nič, da bi ročno omogočili ali aktivirali storitev Rights Management.

Na podlagi povratnih informacij strank ne bomo več omogočali pravil toka pošte za Exchange za samodejno šifriranje odhodne e-pošte, ki vsebuje določeno vrsto občutljivih informacij v vašem najemniku. Namesto tega vam zagotavljamo podrobna navodila, kako lahko to naredite. Dodatne podrobnosti o tem, kako ustvariti prenosno pravilo za šifriranje občutljivih informacij, najdete v [tem članku.](https://aka.ms/OmeEtr)

- Če uporabljate Outlook spletu (prej **OWA):** ko sestavljate e-poštno sporočilo, preprosto **kliknite** Zaščiti v programu OWA. To bo veljalo za dovoljenje »Ne posreduj«. Kliknite **Spremeni dovoljenje in** izberite **Šifriraj,** da šifrirate sporočilo.

- Če **uporabljate Outlook** odjemalca : Če želite poslati šifrirano sporočilo iz programa Outlook 2013 ali 2016 ali Outlook 2016 za Mac, izberite **Možnosti** Dovoljenja , nato pa izberite želeno možnost  >  zaščite.

- Če **želite samodejno šifrirati** vso e-pošto, poslano določenim prejemnikom ali zunanjim partnerskim organizacijam, morate ustvariti pravilo za prenos pošte v skrbniškem središču za Exchange pošte. Podrobna navodila so na voljo v [tem članku s podporo.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

