---
title: Popravljanje pravilnika o povezavi
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314860"
---
# <a name="fix-connection-policy"></a>Popravljanje pravilnika o povezavi

E-pošta je bila označena kot varna in dostavljena v uporabnikovo mapo »Prejeto«, ker je bil izvorni naslov IP v privzetem pravilniku filtra povezave označen kot varen. Če želite pregledati pravilnik, naredite to:

1. V portalu Microsoft 365 Defender v razdelku Pravilniki pojdite na Pravilniki za sodelovanje z <https://security.microsoft.com/>  \>  \>  \> **e-&**  in pravilniki o & za preprečevanje neželene pošte.

   Če se želite neposredno po vrniti na **stran Pravilniki za preprečevanje neželene** pošte, uporabite <https://security.microsoft.com/antispam> .

2. Na strani **Pravilniki za neželeno** pošto izberite pravilnik z imenom Pravilnik filtriranja povezave **(privzeto),** tako da kliknete ime pravilnika.

3. V prikazanem oknu s podrobnostmi kliknite **Urejanje pravilnika filtra** povezave v **razdelku Filtriranje** povezave.

4. Preglejte vnose v razdelku Vedno dovoli sporočila iz **teh naslovov IP** ali obsega naslovov in si oglejte, ali je **izbrana** možnost Vklopi varni seznam.

   **Opomba:** Microsoft se naroči na vire zaupanja vrednih pošiljateljev tretjih oseb. Če je seznam varnih naslovov omogočen, ti zaupanja vredni pošiljatelji niso pomotoma označeni kot neželena pošta. Priporočamo, da to možnost izberete, saj se s tem zmanjša število napačnih pozitivnih pošiljateljev (dobra pošta, ki je razvrščena kot neželena pošta), ki jo prejmete.

Če želite več informacij, [glejte Konfiguracija filtriranja povezave.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
