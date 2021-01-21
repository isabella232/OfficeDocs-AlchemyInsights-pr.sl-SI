---
title: Konfiguracija in podaljšanje življenjske dobe žetona
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917012"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfiguracija in podaljšanje življenjske dobe žetona

Določite lahko življenjsko dobo žetona Accessa, SAML ali ID-ja, ki ga je izdajala Microsoftova platforma za identiteto. Življenjske dobe žetonov lahko nastavite za vse programe v organizaciji, za program multi-najemnika (multi-Organization) ali za določenega glavnega ponudnika v organizaciji. Če želite več informacij, preberite [trajanje veljavnosti žetonov](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes), ki jih je mogoče konfigurirati.

Za primere preberite [primere, kako konfigurirate življenjske dobe žetona](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Če želite izvedeti, kako konfigurirate življenjsko dobo in združljivost žetona v storitvi Azure Active Directory B2C (Azure AD B2C), glejte [Konfiguracija žetonov v storitvi Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

V članku [konfigurirajte delovanje sej v storitvi Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) , v katerem so opisani načini enotne prijave (SSO), ki se uporabljajo v storitvi AZURE ad B2C in vam pomaga pri konfiguraciji pravilnika izbrati najprimernejšo metodo SSO.

**Kako dolgo trajajo žetoni? Kako dolgo veljajo?**

Življenjska doba žetonov je 1 ura in življenjska doba seje je 24 ur. To pomeni, da se boste morali znova prijaviti, preden zaprosite za nov žeton, če v 24 urah ni bilo nobenih zahtev.

> [!NOTE]
> Po maju 30, 2020, noben novi najemnik ne bo mogel uporabiti pravilnika o življenjskem simbolu, ki ga je mogoče konfigurirati za konfiguracijo zasedanja in osveževanja žetonov. Zastaranje se bo zgodilo v nekaj mesecih po tem, kar pomeni, da bomo ustavili čast obstoječega zasedanja in osvežili žetone policije. Po zastaranju lahko še vedno konfigurirate življenjske dobe žetona za dostop.






