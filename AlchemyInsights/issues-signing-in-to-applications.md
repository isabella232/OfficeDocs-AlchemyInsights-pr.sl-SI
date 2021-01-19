---
title: Težave pri vpisu v programe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901325"
---
# <a name="issues-signing-in-to-applications"></a>Težave pri vpisu v programe

Če želite zaznati težave, povezane z uporabniškim vpisom, izvedite te korake:

1. Zaženite [diagnostiko za vpis](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Poiščite dogodek, ki ga želite analizirati, tako da vnesete podrobnosti, ki jih imate o uporabniku, aplikaciji, času vpisa, zahtevi ID-ja ali korelaciji.
3. Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko izvedete, če želite spremeniti spremembe, če so potrebne spremembe.

V nadaljevanju so navedene nekatere pogoste težave, ki se lahko pojavijo pri vpisu v programe:

1. Vi ali uporabnik **dokončate vpis v AZURE ad, vendar se prikaže nepričakovano opozorilo** – glejte članek [nepričakovana privolitev, ko se vpišete](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) v program in [Nepričakovana napaka pri izvajanju dovoljenja za program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Vi ali uporabnik ste se **vpisali v program neposredno, vendar se ne morete vpisati v deeplink na portalu po meri ali v Accessovi plošči**: glejte [Odpravljanje težav pri vpisu v program iz storitve Azure ad My apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Vi ali uporabnik **je dokončal vpis v AZURE ad, vendar aplikacija prikaže sporočilo o napaki in ne dovoli uporabniku, da dokonča vpisni tok**: težava je v tem, da aplikacija ni sprejela odgovora, ki ga je izdal Azure ad. Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) za odpravljanje težav.
4. Vi ali uporabnik se **ne morete vpisati v program, ki ni v galeriji, konfiguriran za enotno prijavo gesla**: upoštevajte navodila v [teh](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) navodilih za odpravljanje težav.
5. Vi ali uporabnik se **ne morete vpisati v galerijo storitve AZURE ad, ki je konfigurirana za enotno prijavo gesla**: Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) za odpravljanje težav.
6. Vi ali uporabnik se **ne morete vpisati v Microsoftov program**: Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) za odpravljanje težav.
7. Vi ali uporabnik se **ne morete vpisati v program, ki ni v galeriji konfiguriran za Združeno enotno prijavo**: Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) za odpravljanje težav.
8. Vi ali uporabnik se **ne morete vpisati v galerijo storitve AZURE ad, ki je konfigurirana za Združeno enotno prijavo**: Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) za odpravljanje težav.
9. Vi ali uporabnik se **ne morete vpisati v program po meri**: Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) za odpravljanje težav.
10. Vi ali uporabnik se **ne morete vpisati v program na mestu uporabe s proxyjem storitve AZURE ad**: Upoštevajte [ta navodila](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) za odpravljanje težav.

