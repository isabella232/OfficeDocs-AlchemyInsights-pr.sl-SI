---
title: Nastavitev DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645688"
---
# <a name="setup-dkim"></a>Nastavitev DKIM

Popolna navodila za konfiguriranje DKIM za domene po meri v Microsoft 365 so [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Za **vsako** domeno po meri morate ustvariti **dva** zapisa DKIM CNAME v storitvi gostovanja DNS domene (običajno registrar domene). Contoso.com in fourthcoffee.com na primer zahtevata štiri zapise DKIM CNAME: dve za contoso.com in dva za fourthcoffee.com.

   Zapisi DKIM CNAME za **vsako** domeno po meri uporabljajo naslednje formate:

   - **Ime gostitelja**:`selector1._domainkey.<CustomDomain>`

     **Točke za naslov ali vrednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ime gostitelja**:`selector2._domainkey.<CustomDomain>`

     **Točke za naslov ali vrednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je besedilo v levem `.mail.protection.outlook.com` zapisu po meri MX za domeno po meri (na primer `contoso-com` za domeno contoso.com). \<InitialDomain\> je domena, ki ste jo uporabili, ko ste se prijavili za Microsoft 365 (na primer contoso.onmicrosoft.com).

2. Ko ustvarite zapise CNAME za domene po meri, izpolnite ta navodila:

   A. [Vpišite se v Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s svojim delovnim ali šolskim računom.

   B. V zgornjem levem kotu izberite ikono zaganjalnika aplikacij in izberite **skrbnik**.

   C. V spodnjem levem krmarjenju razširite možnost **skrbnik** in izberite **Exchange**.

   D. Pojdi na **zaščito** > **DKIM**.

   E. Izberite domeno in nato izberite **Omogoči** za **podpisovanje sporočil za to DOMENO s podpisi DKIM**. Ponovite ta korak za vsako domeno po meri.
