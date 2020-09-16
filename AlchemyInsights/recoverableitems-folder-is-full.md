---
title: Mapa» 1336 RecoverableItems «je polna
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741283"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapa» obnovljivi elementi «je polna

Za nabiralnike v storitvi Exchange Online je privzeta omejitev shrambe za mapo» obnovljivi elementi «30 GB. Omejitev shrambe za mapo» obnovljivi elementi «je samodejno povečana na 100 GB, če je nabiralnik nastavljen na zadržanje zaradi spora, E-odkrivanje zadržanje ali pa je dodeljen pravilniku o hranjenju.

Ko mapa» obnovljivi elementi «doseže omejitev shrambe, vpliva na funkcije nabiralnika na te načine:

- Uporabnik ne more izbrisati elementov iz nabiralnika.

- Pomočnik za upravljane mape ne more izbrisati elementov, ki temeljijo na nastavitvah oznake hranjenja ali upravljanih map.

- Za nabiralnike, ki imajo omogočeno obnovitev enega elementa ali pa so zadržane, proces zaščite pred kopiranjem na mesto pisanja ne more vzdrževati različic elementov, ki jih je uredil uporabnik.

- Za nabiralnike, ki imajo omogočeno pisanje dnevnika nadzora nabiralnika, ni mogoče shraniti vnosov dnevnika nadzora nabiralnika v podmapo» revizije «v mapi» obnovljivi elementi «.

Za nabiralnike, ki niso zadržani, lahko skrbniki z `Search-Mailbox -SearchDumpsterOnly -DeleteContent` ukazom PowerShell za Exchange Online izbrišejo elemente v mapi» obnovljivi elementi «. Če želite več informacij, glejte te teme:

- [Iskanje in brisanje sporočil](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Iskanje nabiralnika](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za nabiralnike, ki so zadržani, morajo skrbniki odstraniti zadržanje, preden lahko izbrišejo elemente iz mape» obnovljivi elementi «. Če želite več informacij, glejte [brisanje elementov v mapi» obnovljivi elementi «nabiralnikov v oblaku v zadržanju](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Če želite preprečiti, da bi se mapa» obnovljivi elementi «ohranila v celoti, lahko skrbniki povečajo omejitev shrambe mape» obnovljivi elementi «za nabiralnike v zadržanju in nastavijo pravilnik o hranjenju nabiralnika, ki premakne elemente iz mape» obnovljivi elementi «v nabiralnik uporabnikovega arhiva. Glejte [povečanje kvote za obnovljive elemente za nabiralnike v zadržanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
