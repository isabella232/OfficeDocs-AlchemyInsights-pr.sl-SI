---
title: Izvoz E-odkrivanje/rezultatov iskanja vsebine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429973"
---
# <a name="export-ediscoverycontent-search-results"></a>Izvoz E-odkrivanje/rezultatov iskanja vsebine

Morda boste morali rezultate iskanja izvoziti v datoteko PST (iz e-pošte) ali v izvorne Officeove dokumente (na mestih SharePoint in OneDrive za podjetja). V tem primeru naredite to:

- Preverite, ali je vaš račun dodeljen ustreznim dovoljenjem za izvoz. Če želite več informacij, glejte [dodeljevanje dovoljenja za e-odkrivanje](https://go.microsoft.com/fwlink/?linkid=2102406).
- Prepričajte se, da je računalnik izpolnjeval vse [pogoje](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin). Vsi brskalniki niso podprti, kot je Chrome.
- Izvoz iz iskanja vsebine: a. Pojdite v [središče za skladnost z varnostnim &](https://protection.office.com/contentsearch) in kliknite **Iskanje**, nato pa izberite **Iskanje vsebine**. Na strani **Iskanje vsebine** Izberite shranjeno iskanje.
    b. V podoknu s podrobnostmi v razdelku **izvoz rezultatov v računalnik** izberite **Zaženi izvozi**. Če izvažate več kot 100K nabiralnike, boste morali uporabiti PowerShell za prenos rezultatov izvoza. Če želite več informacij, glejte [izvažanje rezultatov iz več kot 100k nabiralnikov](https://go.microsoft.com/fwlink/?linkid=2143861).

Če želite izvedeti več, glejte [izvoz rezultatov iskanja vsebine](https://go.microsoft.com/fwlink/?linkid=2102118).