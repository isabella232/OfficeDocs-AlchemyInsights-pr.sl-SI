---
title: Ali so vaši uporabniki prejeli e-pošto z zlonamerno vsebino?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929213"
---
# <a name="did-your-users-receive-malicious-email"></a>Ali so vaši uporabniki prejeli e-pošto z zlonamerno vsebino?

- E-pošto z zlonamerno vsebino lahko odslej prijavite Microsoftu s [skrbniškimi pošiljkami v središču za varnost in skladnost s predpisi](https://sip.protection.office.com/reportsubmission).

Sporočila, ki so poslana v [skrbniških pošiljkah](https://sip.protection.office.com/reportsubmission), so pregledane, v pojavnem oknu s **podrobnostmi** pa so prikazani ti rezultati:

- Če je prišlo do napake v preverjanju pristnosti e-poštnega naslova pošiljatelja ob trenutku dostave.
- Informacije o morebitnih zadetkih pravilnika, ki bi lahko vplivale na odločitev o sporočilu ali pa bi jo preglasile.
- S trenutno detonacijo je prikazano, ali so bili URL-ji ali datoteke, ki so bile v sporočilu, zlonamerne ali ne.
- Povratne informacije ocenjevalcev

Če je bila zaznana preglasitev, bi moral biti v nekaj minutah dokončan vnovični pregled. Če ni prišlo do težave pri preverjanju pristnosti ali če na dostavo ni vplivala preglasitev, bi lahko povratne informacije ocenjevalcev trajale do enega dne.

Če se ne strinjate s končno oceno sporočila, URL-ja ali datoteke (blokirano ali neblokirano), po enem dnevu znova pošljite sporočilo za vnovični pregled. Obstaja velika verjetnost, da bo ocena sporočila po vnovični pošiljki drugačna.

Medtem lahko zlonamerno e-pošto odstranite iz uporabniških nabiralnikov tako, da upoštevate navodila v [tem članku](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Stranke s platformo Microsoft Defender za Office 365 lahko izvajajo ta opravila:
    - uporabijo [Raziskovalca groženj za iskanje in brisanje sumljive e-pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered),
    - [uporabijo Varne povezave za blokiranje dostopa](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) do zlonamernega URL-ja,
    - sledijo uporabnikom, ki so kliknili zlonamerne URL-je in dostopali do njih: [ogled URL-jev lažnega predstavljanja in klik za oceno o podatkih](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace),
    - ročno [začnejo avtomatizirano preiskavo](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).

Lahko tudi uporabite zaščito pred zlonamernimi datotekami in URL-ji tako, da upoštevate navodila v razdelku [Zaščita pred zlonamernimi URL-ji in datotekami](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).