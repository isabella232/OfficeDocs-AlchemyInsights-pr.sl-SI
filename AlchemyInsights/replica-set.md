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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714584"
---
# <a name="replica-set"></a>Nabor replik

AADDS je imenovan tudi kot upravljana domena. To je pravzaprav dva krmilnika domene, ki jih izvaja in vzdržuje backend. Dva DCs vključujeta en glavni DC in en replikacijski DC. Varnostne kopije v AADDS (upravljana domena) so avtomatiziran proces, ki ga upravlja Azure platform. V primeru težave z upravljano domeno vam lahko podpora Azure pomaga pri obnavljanju iz varnostnega kopiranja.

Vsak nabor replik ustvarite v navideznem omrežju. Vsako navidezno omrežje je treba pokukati v vsako drugo navidezno omrežje, ki gosti nabor replik v upravljani domeni. S to konfiguracijo ustvarite topologijo omrežja mesh, ki podpira replikacijo imenika. Navidezno omrežje lahko podpira več naborov replik, pod pogojem, da je vsak nabor replik v drugem navideznem podomrežju.

Če želite več podrobnosti o naboru replik, glejte [nabori pojmov replika](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
