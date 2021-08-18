---
title: Nastavitev kontrolnika DKIM z domenami po meri
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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332323"
---
# <a name="set-up-dkim-with-custom-domains"></a>Nastavitev kontrolnika DKIM z domenami po meri

Objaviti morate dva zapisa CNAME za vsako domeno po meri v sistemu DNS. To naredite tako:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Opomba:** **DomainGUID** je besedilo na levi strani **.mail.protection.outlook.com** v prilagojenem zapisu MX za domeno po meri (na primer contoso-com za domeno **contoso.com**). **InitialDomain** je domena, ki ste jo uporabili, ko ste se prijavili Office 365 (na primer **contoso.onmicrosoft.com**).

Če želite več informacij o zapisih DNS, glejte Ustvarjanje zapisov DNS pri poljubnih ponudnikih [gostovanja DNS za Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)