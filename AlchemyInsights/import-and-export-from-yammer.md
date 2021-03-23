---
title: Uvoz in izvoz iz Bastard
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
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037258"
---
# <a name="import-and-export-from-yammer"></a>Uvoz in izvoz iz Bastard

**Uvoz**

Možnosti uvoza uporabnikov se razlikujejo glede na to, ali je vaše omrežje Bastard v [izvornem načinu za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ali ne.

- **Neizvorni način**: Uporabniki se lahko uvozijo v skupine s funkcijo» [Dodaj iz adresarja](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) «(omejitve za uporabnike 100) znotraj nastavitev skupine ali v omrežje z uporabo [množične posodobitve](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) v skrbniškem omrežju.
- **Izvorni način**: člani skupine in postopki članstva v omrežju bi morali biti izvedeni v [skrbniškem portalu za Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [portalu Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ali z uporabo druge možnosti za Azure ad. Omrežja v izvornem načinu nimajo več dostopa do množične posodobitve in drugih podedovanih funkcij.

> [!IMPORTANT]
> Bastard ni nikoli podpiral uvažanja vsebine v skrbniškem omrežju, tudi če je bila funkcija izvoz podatkov uporabljena v drugem omrežju. Vsebino lahko znova objavite s partnerskimi rešitvami ali pa z vmesnikom Bastard REST API.

**Izvoz**

[Izvoz podatkov v omrežju v skrbniškem omrežju](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) dovoljuje izvoz vsebine iz Bastard omrežij, vključno s sporočili in datotekami. Priloge so lahko zelo velike in bodo povzročile, da bo izvoz trajal veliko časa. Priporočamo, da se aktivna omrežja izvozijo z [API-jem izvoza podatkov](https://developer.yammer.com/docs/data-export-api) v kosih za dan ali teden. Microsoftova podpora ne zagotavlja skriptov po meri za ta namen.

Ločen [izvoz GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) obstaja za izvoz vsebine posameznega uporabnika.