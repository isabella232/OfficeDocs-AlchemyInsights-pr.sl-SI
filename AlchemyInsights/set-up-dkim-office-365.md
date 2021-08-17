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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108572"
---
# <a name="setup-dkim"></a>Nastavitev DKIM

Celotna navodila za konfiguracijo kontrolnika DKIM za domene po meri v Microsoft 365 so [tukaj.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Za **vsako** domeno po meri morate ustvariti dva zapisa **DKIM** CNAME v storitvi gostovanja DNS domene (običajno je to registrator domene). Za contoso.com in fourthcoffee.com na primer potrebujete štiri zapise DKIM CNAME: dva za contoso.com, dva pa za fourthcoffee.com.

   Zapisi DKIM CNAME za **vsako domeno** po meri uporabljajo te oblike zapisa:

   - **Ime gostitelja:**`selector1._domainkey.<CustomDomain>`

     **Kaže na naslov ali vrednost:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (Življenjska** doba): 3600

   - **Ime gostitelja:**`selector2._domainkey.<CustomDomain>`

     **Kaže na naslov ali vrednost:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL (Življenjska** doba): 3600

   \<DomainGUID\> besedilo na levi strani prilagojenega zapisa MX za domeno po meri (na primer za domeno `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>je domena, ki ste jo uporabili, ko ste se prijavili Microsoft 365 (na primer contoso.onmicrosoft.com).

2. Ko ustvarite zapise CNAME za domene po meri, dokončajte ta navodila:

   a. [se vpišite Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s službeim ali šolskim računom.

   b. Izberite ikono zaganjalnika programov v zgornjem levem kotu in izberite **Skrbnik**.

   c. V spodnjem levem podoknu za krmarjenje razširite **razdelek Skrbnik** in **izberite Exchange**.

   d. Pojdite na **Zaščita**  >  **DKIM**.

   e. Izberite domeno in nato **izberite** Omogoči za podpisovanje sporočil za to **domeno s podpisi DKIM.** Ponovite ta korak za vsako domeno po meri.
