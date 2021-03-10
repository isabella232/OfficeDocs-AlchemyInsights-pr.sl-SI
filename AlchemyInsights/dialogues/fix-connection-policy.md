---
title: Popravi pravilnik povezave
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695888"
---
# <a name="fix-connection-policy"></a>Popravi pravilnik povezave

E-pošta je bila označena kot varna in dostavljena v uporabnikovo mapo» Prejeto «, ker je bil naslov IP za pošiljanje v pravilniku filtra povezave označen kot varen. Če želite pregledati pravilnik, naredite to:

1. Obiščite središče za [skladnost s predpisi sistema Office & 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)in nato pojdite na pravilnik za **upravljanje groženj** za  >    >  [preprečevanje neželene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na zavihku **po meri** izberite **pravilnik filtra povezave** in nato izberite **Uredi pravilnik**.
3. Preglejte seznam **dovoljenih IP** . Preverite, ali je omogočen **varni seznam** .

    > [!NOTE]
    > Microsoft je naročen na vire neodvisnih ponudnikov zaupanja vrednih pošiljateljev. Če je omogočeno **varno seznam** , se ti zaupanja vredni pošiljatelji ne zmotno označijo kot neželena pošta. Priporočamo, da izberete to možnost, saj bo zmanjšala število lažnih pozitivnih rezultatov (dobra pošta, ki je razvrščena kot neželena pošta), ki jo prejmete.
