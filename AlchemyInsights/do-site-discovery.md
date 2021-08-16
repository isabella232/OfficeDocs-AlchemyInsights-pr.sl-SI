---
title: Odkrivanje mesta
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030774"
---
# <a name="do-site-discovery"></a>Odkrivanje mesta

Če vaša organizacija še vedno uporablja podedovane spletne programe in načrte za uporabo načina Internet Explorerja (kar večina strank dela), potem morate narediti nekaj dodatnega odkrivanja mesta.

**Starejšo različico programa Microsoft Edge**

Če ste seznam mest podjetja že konfigurirali tako, da deluje za starejšo različico Microsoft Edge, je odkrivanje spletnega mesta skoraj končano. Morda boste morali dodati nevtralna mesta.

Nevtralna mesta so po navadi mesta z enotno prijavo (SSO). Če na nevtralno spletno mesto s Microsoft Edge, želite ostati na mestu in Microsoft Edge pristnosti. Če v načinu Internet Explorerja greste na nevtralno mesto, želite za preverjanje pristnosti ostati v načinu Internet Explorerja.

Določite kateri koli SSO ali druga nevtralna mesta, ki jih uporabljate, in jih dodajte na seznam spletnih mest podjetja.

**Internet Explorer je vaš privzeti brskalnik**

Če trenutno uporabljate le Internet Explorer, morda ne veste, katera mesta so bila nadgrajena na sodobne spletne standarde in za katera še vedno potrebujete Internet Explorer. Ta mesta boste želeli poiskati in jih dodati na seznam mest za podjetja, tako da boste lahko internet explorerski način uporabljali le za ta spletna mesta.

> [!NOTE]
> [Odkrivanje spletnega mesta podjetja](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) odkrije mesta, ki morda potrebujejo način Internet Explorerja. Zbira lahko podatke v računalnikih, v katerih Windows od Internet Explorer 8 do Internet Explorer 11 v sistemih Windows 10, Windows 8.1 ali Windows 7.

**Analiziranje podatkov**

Ko zberete podatke mesta, priporočamo, da za analizo podatkov analizirati ta postopek v štirih korakih:
1. Razvrstite podatke po domeni in nato po URL-ju.
2. Določite meje programa, ki ga želite konfigurirati za način Internet Explorerja. Vključiti želite vsa mesta in spletne kontrolnike, ki določajo program, ne želite pa vključiti dodatnih mest in kontrolnikov. Nekatera spletna mesta so lahko zelo preprosta, medtem ko boste morali druga *https://contoso.com/app1* morda določiti več spletnih mest in strani.
3. Preskusite program in se prepričajte, da ne deluje izvorno. Številna mesta ponujajo sodobno vsebino, ko zaznajo sodobni brskalnik in ponudijo podedovano vsebino le, ko zaznajo Internet Explorer.
4. Če program ne uspe in ne deluje, ga dodajte na seznam mest za podjetja.

> [!NOTE]
> V skladu z najboljšo prakso združite vsa mesta, ki so sestavljena iz aplikacije. Ko na ta način nadgradite program, boste iz načina Internet Explorerja lažje odstranili celotno mesto in za ta program začeli uporabljati sodoben brskalnik.

Ko končate z odkrivanjem mest in analizirate podatke, lahko začnete raziskovati strategijo kanala.

