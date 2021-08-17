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
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893419"
---
# <a name="did-your-users-receive-malicious-email"></a>Ali so vaši uporabniki prejeli e-pošto z zlonamerno vsebino?

Zlonamerno e-pošto lahko zdaj prijavite Microsoftu prek [pošiljanj v Microsoft 365 Defender portalu.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Sporočila, ki so poslana [v skrbniških sporočilih,](https://security.microsoft.com/reportsubmission?viewid=admin) so pregledana, v področju s podrobnostmi pa so prikazani ti rezultati:

- Če je prišlo do napake v preverjanju pristnosti e-poštnega naslova pošiljatelja ob trenutku dostave.
- Informacije o morebitnih zadetkih pravilnika, ki bi lahko vplivale na odločitev o sporočilu ali pa bi jo preglasile.
- S trenutno detonacijo je prikazano, ali so bili URL-ji ali datoteke, ki so bile v sporočilu, zlonamerne ali ne.
- Povratne informacije ocenjevalcev

Če je bila zaznana preglasitev, bi moral biti v nekaj minutah dokončan vnovični pregled. Če ni prišlo do težave pri preverjanju pristnosti ali če na dostavo ni vplivala preglasitev, bi lahko povratne informacije ocenjevalcev trajale do enega dne.

Če se ne strinjate s končno oceno sporočila, URL-ja ali datoteke (blokirano ali neblokirano), po enem dnevu znova pošljite sporočilo za vnovični pregled. Obstaja velika verjetnost, da bo ocena sporočila po vnovični pošiljki drugačna.

Medtem lahko zlonamerno e-pošto odstranite iz uporabniških nabiralnikov tako, da upoštevate navodila v [tem članku](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Stranke s platformo Microsoft Defender za Office 365 lahko izvajajo ta opravila:
  - Uporaba [Raziskovalca groženj za iskanje in brisanje sumljive e-pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Uporaba Sef povezav za blokiranje dostopa do](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) zlonamernega URL-ja
  - Sledenje uporabnikom, ki so kliknili zlonamerne URL-je in dostopali do njih: Ogled [URL-ja](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)z lažnim predstavljanjem in klikanje podatkov za prerekovanje  &  [Get-URLTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Ročni [začetek avtomatizirane raziskave](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Lahko tudi uporabite zaščito pred zlonamernimi datotekami in URL-ji tako, da upoštevate navodila v razdelku [Zaščita pred zlonamernimi URL-ji in datotekami](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
