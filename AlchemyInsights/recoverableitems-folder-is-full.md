---
title: 1336 RecoverableItems mapa je polna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510768"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapa» Obnovljivo «je polna

Za nabiralnike Exchange Online je privzeta omejitev shranjevanja za mapo» Obnovljivo «30 GB. Omejitev shranjevanja za mapo» Obnovljivo «se samodejno poveča na 100 GB, če je nabiralnik postavljen na čakanje zaradi spora, zadržanje e-odkrivanja ali pa je dodeljen pravilniku o hranjenju.

Ko mapa» Obnovljivo «doseže omejitev shranjevanja, je funkcija nabiralnika prizadeta na naslednje načine:

- Uporabnik ne more izbrisati elementov iz nabiralnika.

- Pomočnik za upravljane mape ne more izbrisati elementov, ki temeljijo na oznaki za hranjenje ali v nastavitvah upravljane mape.

- Za nabiralnike, ki imajo omogočeno Obnovitev posameznega artikla ali so dani na voljo, postopek zaščite strani za kopiranje na pisanje ne more vzdrževati različic elementov, ki jih je uredil uporabnik.

- Za nabiralnike, ki imajo omogočeno beleženje dnevnika revizij nabiralnika, ni mogoče shraniti vnosov dnevnika revizij nabiralnika v podmapo revizijah v mapi» obnovljivo «.

Za nabiralnike, ki niso na voljo, lahko skrbniki s pomočjo `Search-Mailbox -SearchDumpsterOnly -DeleteContent` ukaza v PowerShell Exchange Online izbrišejo elemente v mapi» obnovljivo «. Če želite več informacij, glejte naslednje teme:

- [Iskanje in brisanje sporočil](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Iskalni nabiralnik](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za nabiralnike, ki so na zadržani, morajo skrbniki odstraniti zadržko, preden lahko izbrišejo elemente iz mape» Obnovljivo «. Če želite več informacij, glejte [brisanje elementov v mapi» obnovljivo «v nabiralnikih v oblaku, ki jih držite](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Če želite preprečiti, da bi mapa» Obnovljivo «postala polna, lahko skrbniki povečajo omejitev shranjevanja mape» Obnovljivo «za nabiralnike na zadržanju in nastavijo pravilnik o hranjenju nabiralnika, ki premakne elemente iz mape» Obnovljivo «v arhivski nabiralnik uporabnika. Glejte [povečanje kvote za obnovljivo postavko za nabiralnike na zadržanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
