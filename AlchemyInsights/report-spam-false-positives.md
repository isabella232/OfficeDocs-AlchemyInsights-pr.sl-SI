---
title: Ali želite Microsoftu prijaviti napačno pozitivno neželeno pošto?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396631"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Ali so želena sporočila označena kot neželena pošta?

To je neprijetno, če legitimna e-pošta konča v mapi z neželeno pošto ali v karanteni. Upoštevajte te najpogostejše razloge za napačno pozitivno vrednost:

**Preglasitve najemnika (najpogostejše)** To je v celoti na voljo v okviru vašega nadzora, da popravite.

Pošljite sporočilo na Microsoft 365 Defender analizo pravilnikov in pravil, ki vplivajo nanje; so na voljo čez nekaj minut.
Preglejte ali spremenite pravilnike ali pravila, kot so na voljo. 

**Prepisi končnega uporabnika (pogosto)** To je v celoti na voljo v okviru vašega nadzora, da popravite. 

Pošljite sporočilo na Microsoft 365 Defender analizo pravilnikov in pravil, ki vplivajo nanje; so na voljo čez nekaj minut. 

Če je bilo sporočilo blokirano, ker je bilo poslano z naslova na seznamu blokiranih pošiljateljev uporabnika, so v glavah vključeni verdict »SFV:BLK« filtriranja neželene pošte.

**Preverjanje pristnosti e-pošte pošiljateljev** To je delno v okviru vašega nadzora zaradi popravkov.

Pošljite sporočilo, da analizirate napake pri preverjanju pristnosti e-pošte pošiljatelja v času dostave; rezultati so na voljo v enem dnevu. 

Če ste lastnik infrastrukture pošiljanja, preglejte, kako jo uskladite s sistemi SPF, DKIM in DMARC, da zagotovite, da ciljni e-poštni sistemi zaupajo sporočilom, poslanim z vaše domene. Lahko pa tudi stopite v stik s pošiljatelji, ki bodo naslovili konfiguracije SISTEMA DNS.

**Microsoftovo filtriranje verdicts** To je delno v okviru vašega nadzora zaradi popravkov.

Pošljite sporočilo in sporočilo prijavite kot varno; rescan results are available within a day. Seznam allow/block uporabite, ko se ne strinjate s filtriranjem narekovajev v določenih primerih. Vendar pa ne bi smeli zaobiti Microsoftovega filtriranja verdicts trajno. 

Če želite več informacij, si oglejte:

- Omogočite končnim uporabnikom pošiljanje sporočil Microsoftu. Microsoft te oddaje uporabi za izboljšanje učinkovitosti tehnologij za zaščito e-pošte, ki so prikazana med pošiljanjem poročil, ki jih boste uporabili kot namig za posodobitev pravilnikov. 

- Če si želite ogledate kratek videoposnetek o pošiljanju sporočil v analizo, glejte [Pošiljanje sporočil v analizo.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [S pošiljanjem vsebine za skrbnike lahko Microsoftu pošljete sumljivo neželeno pošto, url-je, URL-je in datoteke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Upravljanje seznama allow/block za najemnika](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Glave sporočil za preprečevanje neželene pošte v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Zaščita pred odhodno pošto v EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)