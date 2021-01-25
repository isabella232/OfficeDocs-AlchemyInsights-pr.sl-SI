---
title: Dovoljenja za API in soglasja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974994"
---
# <a name="api-permissions-and-consent"></a>Dovoljenja za API in soglasja

Programi, ki se integrirajo s platformo Microsoft Identity, spremljajo model avtorizacije, ki uporabnikom in skrbnikom omogoča nadzor nad tem, kako je mogoče dostopati do podatkov. Izvajanje modela odobritve je bilo posodobljeno na končni točki Microsoftove platforme za identiteto. Spreminja, kako mora program delovati z Microsoftovo platformo Identity. [Dovoljenja in soglasje v končni točki Microsoftovega izhodišča identitete](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) so osnovni pojmi tega modela odobritve, vključno z obsegi, dovoljenji in soglasjem.

[Okvir soglasja Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) omogoča preprosto razvijanje spletnih in odjemalskih programov za več najemnikov. Ti programi dovoljujejo vpis s strani uporabniških računov iz strežnika Azure AD najemnika, ki je drugačen od tistega, v katerem je program registriran. Poleg svojih spletnih vmesnikov API lahko tudi potrebujejo dostop do spletnih vmesnikov API, kot je Microsoft Graph API (za dostop do storitev Azure AD, InTune in storitve Microsoft 365) in drugih API-jev Microsoftovih storitev.

