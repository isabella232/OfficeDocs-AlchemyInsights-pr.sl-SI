---
title: Uporaba orodja za uvajanje sistema Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085848"
---
# <a name="using-the-office-deployment-tool-odt"></a>Uporaba orodja za uvajanje sistema Office (ODT)

Z orodjem za uvedbo sistema Office (ODT) lahko uvedete Office 365 različice Officea. Orodje za uvajanje sistema Office (setupodt.exe) se izvaja v ukazni vrstici in uporablja datoteko konfiguracijske datoteke XML, da določi, katere nastavitve uporabiti pri uvajanju Officea.
  
1. Prenesite najnovejšo različico orodja za uvedbo sistema Office iz [Microsoftovega središča za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Z [orodjem za prilagajanje sistema Office (okt)](https://config.office.com) izberite nastavitve uvajanja in ustvarite datoteko XML za konfiguracijo. Izvozite konfiguracijsko datoteko in jo postavite na lokalno mesto v isti mapi, kjer setupodt.exe prebiva.

    **Opomba:** Težave z namestitvijo Officea se običajno pojavijo zaradi napačno konfiguriranih ali malformatted konfiguracijskih datotek. Če se želite izogniti takim težavam, vam priporočamo, da ustvarite konfiguracijsko datoteko z orodjem za prilagajanje sistema Office. Obstoječe konfiguracijske datoteke lahko uvozite tudi v Officeovo orodje za prilagajanje.

3. V ukazu» visok ukazni poziv «preklopite na mesto, kjer setupodt.exe prebiva, in zaženite orodje za uvajanje sistema Office v načinu za prenos in določite konfiguracijsko datoteko, ki ste jo pravkar shranili. V tem primeru je konfiguracijska datoteka imenovana Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. zaženite orodje za uvedbo sistema Office v načinu Konfiguriraj in določite konfiguracijsko datoteko.

```setupodt.exe /configure Configuration.xml```

**Opomba:** Ta korak morate zagnati iz odjemalskega računalnika, v katerem želite namestiti Office, in morate imeti dovoljenja lokalnih skrbnikov v tem računalniku.

Če želite izvedeti več o uporabi orodja za uvajanje sistema Office za aplikacije Microsoft 365 apps za uvajanje, glejte [pregled orodja za uvedbo sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Če želite več informacij o uporabi orodja za prilagajanje sistema Office, glejte [pregled orodja za prilagajanje sistema Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
