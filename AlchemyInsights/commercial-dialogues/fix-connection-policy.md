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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888422"
---
# <a name="fix-connection-policy"></a>Popravljanje pravilnika o povezavi

E-pošta je bila označena kot varna in dostavljena v uporabnikovo mapo »Prejeto«, ker je bil izvorni naslov IP v privzetem pravilniku filtra povezave označen kot varen. Če želite pregledati pravilnik, naredite to:

1. V portalu Microsoft 365 Defender v razdelku Pravilniki pojdite na Pravilniki za <https://security.microsoft.com/> **sodelovanje z e-&** in & pravilniki o \>  \>  \>  grožnjah za **neželeno** pošto.

   Če se želite neposredno po vrniti na **stran Pravilniki za preprečevanje neželene** pošte, uporabite <https://security.microsoft.com/antispam> .

2. Na strani **Pravilniki za neželeno** pošto izberite pravilnik z imenom Pravilnik filtriranja povezave **(privzeto),** tako da kliknete ime pravilnika.

3. V prikazanem oknu s podrobnostmi kliknite **Urejanje pravilnika filtra** povezave v **razdelku Filtriranje** povezave.

4. Preglejte vnose v razdelku Vedno dovoli sporočila iz **teh naslovov IP** ali obsega naslovov in si oglejte, ali je **izbrana** možnost Vklopi varni seznam.

   > [!NOTE]
   > Microsoft se naroči na vire zaupanja vrednih pošiljateljev tretjih oseb. Če je seznam varnih naslovov omogočen, ti zaupanja vredni pošiljatelji niso pomotoma označeni kot neželena pošta. Priporočamo, da to možnost izberete, saj se s tem zmanjša število napačnih pozitivnih pošiljateljev (dobra pošta, ki je razvrščena kot neželena pošta), ki jo prejmete.

Če želite več informacij, [glejte Konfiguracija filtriranja povezave.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
