---
title: Uporaba orodja Office uvajanja
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083786"
---
# <a name="using-the-office-deployment-tool-odt"></a>Uporaba orodja Office uvajanja (ODT)

Z orodjem Office deployment Deployment Tool (ODT) Office 365 nove različice Office. Orodje Office Deployment Tool (setup.exe) se zažene iz ukazne vrstice in s konfiguracijsko datoteko XML določi, katere nastavitve bodo veljale pri uvedbi sistema Office.
  
1. Prenesite najnovejšo različico orodja za Office za uvedbo z Microsoftovega centra [za prenose.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Z [orodjem za Office (OCT)](https://config.office.com) izberite nastavitve uvajanja in ustvarite konfiguracijsko datoteko XML. Izvozite konfiguracijsko datoteko in jo shranite lokalno v isto mapo, kjer setup.exe shranjena.

    **Opomba:** Office do težav z namestitvijo pogosto pride zaradi napačno konfiguriranih ali napačno oblikovanih konfiguracijskih datotek. Če se želite izogniti takšnim težavam, priporočamo, da za ustvarjanje konfiguracijske datoteke Office orodje za prilagajanje konfiguracije. Obstoječe konfiguracijske datoteke lahko uvozite tudi v Office za prilagajanje.

3. V ukaznem pozivu na skrbniški ravni preklopite na mesto, kjer se nahaja setup.exe, in zaženite orodje za uvedbo sistema Office v načinu prenosa ter določite konfiguracijsko datoteko, ki ste jo pravkar shranili. V tem primeru se konfiguracijska datoteka imenuje Configuration.xml:

```setup.exe /download Configuration.xml```

4.Zaženite orodje Office za uvedbo v načinu konfiguracije in določite konfiguracijsko datoteko.

```setup.exe /configure Configuration.xml```

**Opomba:** Ta korak morate zagnati iz odjemalskega računalnika, v katerega želite namestiti Office in imeti v tem računalniku lokalna skrbniška dovoljenja.

Če želite izvedeti več o uporabi Office uvajanja za scenarije Programi Microsoft 365 za podjetja uvajanju, glejte Pregled [orodja za Office uvedbe.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Če želite več informacij o uporabi orodja Office prilagajanja, glejte [Pregled orodja Office prilagajanja.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
