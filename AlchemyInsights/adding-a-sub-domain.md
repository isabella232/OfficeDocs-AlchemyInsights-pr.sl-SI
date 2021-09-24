---
title: Dodajanje pod domene
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506770"
---
# <a name="adding-a-sub-domain"></a>Dodajanje pod domene

Pod domains can be added to the same or a different tenant than the parent domain. V obeh primerih morate upravljati lastne nastavitve DNS na spletnem mestu registratorja. Če ste Microsoftu dovolili, da upravlja vaše nastavitve DNS z zapisi NS, ali če ste kupili domeno pri Microsoftu, ne morete dodati poddomen, ne da bi to prej spremenili.

Najprej dodajte nadrejeno domeno in nato dodajte pod domeno. Če je poddomena v istem najemniku, ni treba dodatno preverjati. Če dodate pod domeno v ločenega najemnika, je zapis DNS txt potreben za preverjanje lastništva, preden dodate domeno in dodatne zapise DNS za izbrane storitve.

- Če želite dodati domeno ali poddomeno, upoštevajte navodila v čarovniku za dodajanje domene ali ročno dodajte domeno ali poddomeno tako, da se odpre nastavitev domene [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)  >    >  **Dodaj domeno.**

Po potrebi:

- Če želite spremeniti, kdo upravlja nastavitve DNS za obstoječo domeno, **pojdite** na Nastavitve Domene , potrdite polje ob domeni, nato pa izberite Manage DNS  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **(Upravljanje zapisov DNS).** V čarovniku izberite **Dodajte svoje zapise DNS in** dokončajte čarovnika.
- Če želite v Domeno, ki jo je kupil Microsoft, dodati pod domain, najprej prenesite domeno k drugemu registratorju, nato pa naredite zgornjo spremembo, da boste lahko upravljali svoje zapise DNS. Navodila najdete v [članku Prenos domene iz Microsofta v drugega gostitelja.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Če prejmete napako, da vašo domeno že uporabljajo drugi člani ali ljudje v vaši organizaciji, boste morali najprej prevzeti ta neu upravljanje računa, preden boste lahko uporabljali domeno. Če želite navodila, [glejte Prevzem neu skrbnika imenika v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
