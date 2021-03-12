---
title: Popravi pravilnik najemnika (preglasitev dejanja)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748988"
---
# <a name="fix-tenant-policy-action-override"></a>Popravi pravilnik najemnika (preglasitev dejanja)

To sporočilo je vplivalo na pravilnik proti neželene pošte v najemniku. Če želite pregledati pravilnik, naredite to:

1. Obiščite središče za [skladnost s predpisi sistema Office & 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)in nato pojdite na pravilnik za **upravljanje groženj** za  >    >  [preprečevanje neželene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Preverite, ali je v **viru pravilnika** prikazano to:  **Add-Xheader/ModifySubject/preusmeritev/brisanje/brez dejanja/SKP**

    Če je tako, na zavihku **po meri** preverite nastavitve pravilnika, ki je prizadelo sporočilo. Možno je, da so **standardne nastavitve** , uporabljene za vse uporabnike storitve Exchange Online, vplivale na sporočilo.

Če želite več informacij o konfiguriranju pravilnikov za filtriranje neželene pošte, glejte [Konfiguracija pravilnikov za filtriranje neželene](https://go.microsoft.com/fwlink/?linkid=2101431)pošte.
