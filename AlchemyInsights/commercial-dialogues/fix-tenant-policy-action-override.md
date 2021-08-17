---
title: Popravljanje pravilnika najemnika (preglasitev dejanja)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896091"
---
# <a name="fix-tenant-policy-action-override"></a>Popravljanje pravilnika najemnika (preglasitev dejanja)

Na to sporočilo je vplival eden od pravilnikov za preprečevanje neželene pošte. Če želite pregledati pravilnike, naredite to:

1. V portalu Microsoft 365 Defender v razdelku Pravilniki pojdite na Pravilniki za <https://security.microsoft.com/> **sodelovanje z e-&** in & pravilniki o \>  \>  \>  grožnjah za **neželeno** pošto.

   Če se želite neposredno po vrniti na **stran Pravilniki za preprečevanje neželene** pošte, uporabite <https://security.microsoft.com/antispam> .

2. Na strani **Pravilniki** za preprečevanje neželene pošte izberite pravilnik tako, da  kliknete ime pravilnika **(** Vrsta je Pravilnik o neželeni pošti po meri ali Ime je Dohodni pravilnik za neželeno pošto **(privzeto)**). 
3. V prikazanem oknu s podrobnostmi izberite **Uredi dejanja** v **razdelku** Dejanja.
4. V razdelku Dejanja **sporočila** preglejte narekovanje za neželeno pošto  **,** neželeno pošto z visoko stopnjo zanesljivosti **,** lažno predstavljanje in lažno predstavljanje z visoko stopnjo zanesljivosti, da vidite, ali so izbrane te vrednosti: 
   - **Dodajanje glave X**
   - **Prepiša vrstico z zadevo z besedilom**
   - **Preusmeri sporočilo na e-poštni naslov**
   - **Izbriši sporočilo**
   - **Brez dejanja**

   Mogoče je, da so standardne **nastavitve, uporabljene** za vse Exchange Online Protection to sporočilo vplivale.

Če želite več informacij, glejte [Konfiguracija pravilnikov za preprečevanje neželene pošte v EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
