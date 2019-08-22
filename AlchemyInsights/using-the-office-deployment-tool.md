---
title: Z orodjem za uvajanje urad
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531591"
---
# <a name="using-the-office-deployment-tool-odt"></a>Z orodjem za uvajanje Officea (ODT)

Uporabite orodje Office uvajanja (ODT) za uvedbo Office 365 različice Officea. Orodjem za uvajanje Officea (setup.exe) izvaja iz ukazne vrstice in uses a konfiguracijske datoteke XML odločiti kaj nastavitve uporabiti pri uvajanju urad.
  
1. Prenesite najnovejšo različico Office uvajanje orodja iz [Microsoftovega centra za prenose](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Uporabite [Office Customization Tool (ČDO)](https://config.office.com) izberite nastavitve uvajanja in ustvarjanje konfiguracijske datoteke XML. Izvozi konfiguracijsko datoteko in jo postavite lokalno na isti mapi, setup.exe, kjer prebiva.

    **Opomba:** Urad umestitev, pogosto pride do težav zaradi da narobe ali konfiguracijske datoteke malformatted. Izogibati se taka vprašanja, vam priporočamo, da uporabite Office Customization Tool ustvarite konfiguracijsko datoteko. Lahko tudi uvozite obstoječe konfiguracijske datoteke Office Customization Tool.

3. Iz visok zapoved uren, preklopite na mestu, kjer setup.exe in zagon orodja za uvajanje urad v travnato gričevje način in določite konfiguracijske datoteke, ki jo pravkar shranili. V tem primeru je zunanja podoba pila imenovan Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Zaženite orodje za uvajanje urad v oblikovati način in določite konfiguracijske datoteke.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Opomba:** Ta korak morate zagnati odjemalskega računalnika, na katerem želite namestiti Office in v računalniku morate imeti lokalne skrbniške pravice.

Če želite izvedeti več o uporabi Officea uvajanje orodja za Office 365 ProPlus scenarijev uvajanja, si oglejte [pregled urad uvajanje orodja](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Za več podrobnosti o tem, kako uporabiti Office Customization Tool, si oglejte [pregled Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
