---
title: Nastavitev DKIM v Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765429"
---
# <a name="setup-dkim-in-office-365"></a>Nastavitev DKIM v Office 365

Celotna navodila za konfiguracijo DKIM za custom domene v Office 365 so [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Za **vsako** domeno, po meri, morate ustvariti **dva** DKIM CNAME zapisi na vaše domene DNS gostovanje storitev (praviloma registratorja domene). Na primer contoso.com in fourthcoffee.com zahtevajo štiri zapise DKIM CNAME: dve za contoso.com in dva za fourthcoffee.com.

   DKIM CNAME zapisov za **vsako** domeno po meri uporabite naslednje formate:

   - **Ime gostitelja**:`selector1._domainkey.<CustomDomain>`

     **Točki naslov ali vrednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ime gostitelja**:`selector2._domainkey.<CustomDomain>`

     **Točki naslov ali vrednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je besedilo levo od `.mail.protection.outlook.com` v prilagojeno zapis MX za domeno po meri (na primer, `contoso-com` za domeno contoso.com). \<InitialDomain\> je domena, ki ste ga uporabili, ko ste se prijavili za program Office 365 (na primer, contoso.onmicrosoft.com).

2. Ko ustvarite zapise CNAME za custom domene, izpolnite naslednja navodila:

   a. [Prijavite se v Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) z računom delo ali v šolo.

   b. Izberite ikono app pobudnik v zgornjem desnem in izberite **Admin**.

   c. V spodnjem levem navigacija, razširite **Admin** in izberite **izmenjavo**.

   d. Pojdi na **varstvo** > **DKIM**.

   e. Izberite domeno in izberite **Omogoči** za **znak sporočila za to domeno z DKIM podpisov**. Ponovite ta korak za vsako domeno po meri.
