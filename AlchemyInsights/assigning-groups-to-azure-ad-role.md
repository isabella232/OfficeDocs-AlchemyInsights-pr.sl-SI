---
title: Dodeljevanje skupin v vlogo Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885398"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Dodeljevanje skupin v vlogo Azure AD

Če želite dodeliti skupino oglasov Azure ad z izvorom avtoritete v storitvi Azure AD na vlogo v storitvi Azure AD, izvedite te korake:

1. Ustvarjanje nove skupine – če želite ustvariti novo skupino:

    v. Vpišite se v skrbniško središče za Azure AD s **privilegiranim skrbnikom za vloge** ali **globalnimi skrbniškimi** dovoljenji.
    b. Izberite **Azure Active Directory > skupine > vse skupine > novo skupino**.
    c. Ustvarite skupino.

2. Dodelite vlogo skupini bodisi med ustvarjanjem skupine ali ko je skupina ustvarjena.

    v. Če želite skupini dodeliti vlogo v času ustvarjanja skupine, lahko v skupino dodelite vloge preklopnega programa **AZURE ad** in ustvarite skupino.
    b. Če želite skupini dodeliti vlogo, ko je bila ustvarjena, se pomaknite do zavihka **dodeljene vloge** za novo ustvarjeno skupino in dodelite vlogo skupini.  

**Upravljanje članstva v skupini, ki je dodeljena vlogi storitve Azure AD**

Če želite preprečiti dviganje privilegijev, lahko privzeti skrbniki, ki so dodeljeni vlogi, spremenijo le privilegirane skrbnike vlog in globalni skrbniki. Lahko pa se odločijo, da bodo dodeljene lastniku za to skupino in da prenesejo to opravilo.

Če želite več podrobnosti o dodeljevanju skupin v oblaku za vloge v storitvi Azure AD, [si oglejte Dodeljevanje vlog v skupini Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Če želite več informacij o odpravljanju težav, dodeljenih skupinam v oblaku, glejte [Odpravljanje težav z vlogami, dodeljenimi skupinam v oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





