---
title: Indikatorji ne delujejo z brskalnikom Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887456"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatorji ne delujejo z brskalnikom Edge

Ko ustvarite indikator, ga Edge ne spoštuje (Smartscreen). Če želite več informacij, [glejte Ustvarjanje indikatorjev za NASLOVE IP in URL-je/domene.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. korak: Prepričajte se, da:

- Preverite, ali je indikator pravilen (ni tipkarskih napak v NASLOVU IP, pravilno dejanje, pravilne skupine RBAC).
- Ko ustvarite indikator, počakajte najmanj 2 uri, da upoštevate morebitno zakasnitev.
- Preverite, ali so sistemi v Microsoft Defender for Endpoint zdaj na voljo.
- Preverite, ali lahko sistem(i) komunicira z oblakom.
- Preverite, ali je Smartscreen omogočen in dosegljiv, tako da se pomnete na [preskusno mesto](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. korak: Odpravljanje morebitne težave

- Prepričajte se, da odjemalec izpolnjuje zahteve. Če želite podrobnosti, [glejte Ustvarjanje indikatorjev za NASLOVE IP in URL-je/domene.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Preverite, ali uporabljate najnovejšo različico brskalnika Edge. Če želite izvedeti, katero najnovejšo različico imate, [glejte Ugotovite, katero Microsoft Edge imate.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Znova zaženite brskalnik Edge.
- Premaknite se na mesto, za katerega ste nastavitvijo indikator. Če mesto ni prikazano v skladu s pričakovanji, nadaljujte s 3. korakom. 

## <a name="step-3-collect-data"></a>3. korak: Zbiranje podatkov

- **Zberite diagnostične podatke MDEClientAnalyzer.** Navodila najdete v članku [Težave s računalniki za namestitev v Microsoft Defender za končno točko.](issues-with-onboarding-machines.md)
- Če vam je všeč namestitev in zbiranje sledenja aplikaciji Fiddler, glejte [Telerik Fiddler.](http://www.telerik.com/fiddler)
- Če raje uporabljate navodila Microsoftove podpore, izberite spodnjo ikono podpora, da odprete primer podpore.
