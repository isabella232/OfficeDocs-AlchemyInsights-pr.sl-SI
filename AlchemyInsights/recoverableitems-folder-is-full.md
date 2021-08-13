---
title: 1336 RecoverableItems folder is full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061772"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapa »Obnovljivi elementi« je polna

Za Exchange Online nabiralnike je privzeta omejitev shrambe za mapo »Obnovljivi elementi« 30 GB. Omejitev shrambe za mapo »Obnovljivi elementi« se samodejno poveča na 100 GB, če je nabiralnik zadržan zaradi spora, zadržanje e-odkrivanja ali je dodeljen pravilniku o hranjenju.

Ko mapa »Obnovljivi elementi« doseže omejitev prostora za shranjevanje, vplivate na delovanje nabiralnika na te načine:

- Uporabnik ne more izbrisati elementov iz nabiralnika.

- Pomočnik za upravljane mape ne more izbrisati elementov na podlagi oznake za hranjenje ali nastavitev upravljane mape.

- Za nabiralnike, v katere je omogočena obnovitev enega elementa ali so bili zadržati, postopek zaščite strani za kopiranje na pisanje ne more ohraniti različic elementov, ki jih je uredil uporabnik.

- Za nabiralnike, za katere je omogočeno pisanje dnevnika nadzora nabiralnika, vnosov v dnevnik nadzora nabiralnika ni mogoče shraniti v podmapo »Nadzor« v mapi »Obnovljivi elementi«.

Za nabiralnike, ki niso na čakanju, lahko skrbniki z ukazom iz Exchange Online PowerShell izbrišejo elemente v mapi `Search-Mailbox -SearchDumpsterOnly -DeleteContent` »Obnovljivi elementi«. Če želite več informacij, glejte te teme:

- [Iskanje in brisanje sporočil](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za nabiralnike, ki so na čakanju, morajo skrbniki odstraniti zadržanje, preden lahko izbrišejo elemente iz mape »Obnovljivi elementi«. Če želite več informacij, glejte Brisanje elementov v mapi »Obnovljivi elementi« v [zadržanju nabiralnikov v oblaku.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Skrbniki lahko preprečujejo, da bi mapa »Obnovljivi elementi« postala polna, zato lahko povečajo omejitev shrambe mape »Obnovljivi elementi« za zadržane nabiralnike in nastaviti pravilnik o hranjenju nabiralnika, ki premakne elemente iz mape »Obnovljivi elementi« v nabiralnik arhiva uporabnika. Glejte [Povečanje količinske omejitve količinsko omejitev »Obnovljivi elementi« za nabiralnike na čakanju.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
