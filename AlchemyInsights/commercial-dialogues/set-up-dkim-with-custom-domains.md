---
title: Nastavitev DKIM s domenami po meri
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747636"
---
# <a name="set-up-dkim-with-custom-domains"></a>Nastavitev DKIM s domenami po meri

Za vsako domeno po meri v storitvi DNS morate objaviti dva zapisa CNAME. To naredite tako, da uporabite to obliko zapisa:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** je besedilo levo od **. mail.Protection.Outlook.com** v prilagojenem zapisu MX za domeno po meri (na primer contoso-com za domeno **contoso.com**). **InitialDomain** je domena, ki ste jo uporabili, ko ste se prijavili za Office 365 (na primer **contoso.onmicrosoft.com**).

Če želite več informacij o zapisih DNS, si oglejte [Ustvarjanje zapisov DNS pri katerem koli ponudniku gostovanja DNS za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).