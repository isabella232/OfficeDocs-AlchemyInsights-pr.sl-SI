---
title: Nabor replik
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110696"
---
# <a name="replica-set"></a>Nabor replik

AADDS se imenuje tudi upravljana domena. Pravzaprav gre za dva kontrolnika domene, ki se izvajata in vzdržujeta s hrbtno stranjo. Dva DCs vključujeta en glavni DC in en dc za podvajanje. Varnostne kopije v storitvi AADDS (upravljana domena) so avtomatiziran postopek, ki ga upravlja platforma Azure. Če pride do težave z upravljano domeno, vam lahko podpora Azure pomaga pri obnavljanju iz varnostne kopije.

Vsak nabor replik lahko ustvarite v navideznem omrežju. Vsako navidezno omrežje mora biti vzajemno z vsakim navidezno omrežjem, ki gosti nabor replik upravljane domene. S to konfiguracijo ustvarite topologijo omrežja mreže, ki podpira podvajanje imenika. Navidezno omrežje lahko podpira več naborov replik, vendar pod pogojem, da je vsak nabor replik v drugem navideznem podomrežju.

Če želite več podrobnosti o naboru replikacij, glejte [Koncepti naborov replik.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
