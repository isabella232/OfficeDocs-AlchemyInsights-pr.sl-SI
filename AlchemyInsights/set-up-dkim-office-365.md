---
title: Nastavitev DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808723"
---
# <a name="setup-dkim"></a>Nastavitev DKIM

Dokončana navodila za konfiguriranje DKIM za domene po meri v storitvi Microsoft 365 so [tukaj](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Za **vsako** domeno po meri morate ustvariti **dva** DKIM zapisa CNAME pri ponudniku storitev gostovanja DNS domene (običajno je Registrator domene). Na primer contoso.com in fourthcoffee.com zahtevajo štiri zapise CNAME DKIM: dva za contoso.com in dve za fourthcoffee.com.

   Zapisi CNAME DKIM za **vsako** domeno po meri uporabljajo te oblike zapisa:

   - **Ime gostitelja**: `selector1._domainkey.<CustomDomain>`

     **Pokaže na naslov ali vrednost**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ime gostitelja**: `selector2._domainkey.<CustomDomain>`

     **Pokaže na naslov ali vrednost**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je besedilo levo od `.mail.protection.outlook.com` zapisa prilagojene MX za domeno po meri (na primer `contoso-com` za domeno contoso.com). \<InitialDomain\> je domena, ki ste jo uporabili, ko ste se prijavili za Microsoft 365 (na primer contoso.onmicrosoft.com).

2. Ko ustvarite zapise CNAME za domene po meri, dokončajte ta navodila:

   v. [Vpišite se v Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s službenim ali šolskim računom.

   b. Izberite ikono zaganjalnika programov v zgornjem levem kotu in izberite **skrbnik**.

   c. V spodnjem levem podoknu za krmarjenje razširite možnost **skrbnik** in izberite **Exchange**.

   d. Pojdite v razdelek **zaščita**  >  **DKIM**.

   e. Izberite domeno in nato izberite **Omogoči** za **podpisovanje sporočil za to domeno s podpisi DKIM**. Ponovite ta korak za vsako domeno po meri.
