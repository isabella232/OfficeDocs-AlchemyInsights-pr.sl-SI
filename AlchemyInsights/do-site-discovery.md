---
title: Do odkrivanja mesta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694557"
---
# <a name="do-site-discovery"></a>Do odkrivanja mesta

Če vaša organizacija še vedno uporablja podedovane spletne programe in načrte za uporabo programa Internet Explorer (ki ga večina strank naredi), naredite nekaj dodatnega odkrivanja mesta.

**Uvedli ste že starejšo različico programa Microsoft Edge**

Če ste seznam mesta podjetja že konfigurirali tako, da delate za starejšo različico programa Microsoft Edge, je odkrivanje mesta skoraj končano. Eno stvar, ki jo boste morda morali narediti, je dodajanje nevtralnih mest.

Nevtralna mesta so običajno spletna mesta, ki zagotavljajo enotno prijavo (SSO). Če se na spletnem mestu Microsoft Edge pogovorite z nevtralnim mestom, potem želite za preverjanje pristnosti ostati v programu Microsoft Edge. Če se v načinu Internet Explorerja pogovorite z nevtralnim mestom, lahko v načinu Internet Explorerja ohranite preverjanje pristnosti.

Identificirajte katero koli SSO ali druga nevtralna mesta, ki jih uporabljate, in jih dodajte na seznam mesta podjetja.

**Internet Explorer je vaš privzeti brskalnik**

Če uporabljate le Internet Explorer, morda ne veste, katera spletna mesta so nadgradila na sodobne spletne standarde in ki še vedno zahtevajo Internet Explorer. Na seznamu mesta podjetja boste želeli poiskati in dodati ta mesta, da boste lahko uporabljali le način Internet Explorerja le za ta spletna mesta.

> [!NOTE]
> [Odkrivanje](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) spletnih mest za podjetja odkrije spletna mesta, ki bi morda potrebovala način Internet Explorerja. S programom Internet Explorer 11 v sistemu Windows 10, Windows 8,1 ali Windows 7 lahko zbira podatke v računalnikih, v katerih je nameščen Windows Internet Explorer 8.

**Analiziranje podatkov**

Ko zberete podatke o mestu, vam priporočamo, da analizirate podatke s temi štirimi koraki:
1. Razvrščanje podatkov po domeni in nato prek URL-ja.
2. Določite meje programa, ki ga želite konfigurirati za način Internet Explorerja. Želite vključiti vsa spletna mesta in kontrolnike za splet, ki določajo aplikacijo, ne želite pa vključiti dodatnih mest in kontrolnikov. Nekatera spletna mesta so morda tako preprosta, kot *https://contoso.com/app1* bi lahko drugi zahtevali, da določite več mest in strani.
3. Preskusite aplikacijo, da preverite, ali ne deluje izvorno. Številna spletna mesta ponujajo sodobno vsebino, ko zaznajo sodoben brskalnik in ponudijo le podedovano vsebino, ko zaznajo Internet Explorer.
4. Dodajte program na seznam mesta podjetja, če ne testirate.

> [!NOTE]
> Kot najboljšo prakso združite vsa spletna mesta, ki vključujejo program. Ko nadgradite program, boste lažje odstranili celotno mesto iz načina Internet Explorerja in začeli uporabljati sodoben brskalnik za ta program.

Ko končate z odkrivanjem mesta in analizirate podatke, si lahko ogledate strategijo kanala.

