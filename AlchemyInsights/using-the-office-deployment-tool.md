---
title: Uporaba Officeovega orodja za uvajanje
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010886"
---
# <a name="using-the-office-deployment-tool-odt"></a>Uporaba orodja za uvajanje Officea (ODT)

Officeovo orodje za razmestitev (ODT) uporabite za uvajanje Officeovih različic 365. Officeovo orodje za razmestitev (setup. exe) se zažene iz ukazne vrstice in uporablja konfiguracijsko datoteko XML, da določi, katere nastavitve naj se uporabijo pri uvajanju Officea.
  
1. Prenesite najnovejšo različico orodja za uvajanje Officea iz [Microsoftovega centra za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Z [orodjem za prilagajanje Office (Oct)](https://config.office.com) izberite nastavitve uvajanja in ustvarite KONFIGURACIJSKO datoteko XML. Izvozite konfiguracijsko datoteko in jo postavite lokalno v isto mapo, kjer se nahaja setup. exe.

    **Opomba:** Težave z namestitvijo Officea se pogosto pojavijo zaradi napačnih konfiguriranih ali nepravilno oblikovanih konfiguracijskih datotek. Da bi se izognili takim težavam, priporočamo, da za ustvarjanje konfiguracijske datoteke uporabite orodje Office customization Tool. Obstoječe konfiguracijske datoteke lahko uvozite tudi v orodje za prilagajanje Officea.

3. Iz povišanega ukaznega poziva preklopite na mesto, kjer se nahaja setup. exe, in zaženite orodje za uvajanje Officea v načinu prenosa in določite konfiguracijsko datoteko, ki ste jo pravkar shranili. V tem primeru je konfiguracijska datoteka imenovana konfiguracija. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Zaženite orodje za uvajanje Officea v načinu konfiguriranja in določite konfiguracijsko datoteko.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Opomba:** Ta korak morate zagnati v odjemalskem računalniku, v katerem želite namestiti Office, in v tem računalniku morate imeti dovoljenja lokalnega skrbnika.

Če želite izvedeti več o uporabi Officeovega orodja za uvajanje za Microsoft 365 aplikacije za scenarije uvajanja za podjetja, glejte [pregled orodja za uvajanje Officea](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Če želite več podrobnosti o uporabi orodja za prilagajanje Office, glejte [pregled orodja za prilagajanje Officea](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
