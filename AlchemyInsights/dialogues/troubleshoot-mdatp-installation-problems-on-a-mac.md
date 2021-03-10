---
title: Odpravljanje težav z namestitvijo MDATP v računalniku Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696096"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Odpravljanje težav z namestitvijo MDATP v računalniku Mac

Če Ročna namestitev ni uspešna, se na strani s **povzetkom** čarovnika za namestitev prikaže to sporočilo o napaki:

» Prišlo je do napake med namestitvijo. Namestitveni program je zaznal napako, zaradi katere namestitev ni uspela. Za pomoč se obrnite na izdelovalca programske opreme. "

Za uvajanje MDM na strani je prikazana tudi splošna napaka namestitve.

Čeprav ne prikazujemo natančnih napak za končne uporabnike, bomo obdržali dnevniško datoteko z napredkom namestitve v **/Library/Logs/Microsoft/mdatp/install.log**. Vsako sejo namestitve priloži tej dnevniški datoteki. Če želite izključiti le zadnjo sejo namestitve, uporabite `sed` .

Če želite izvedeti več, glejte [Odpravljanje težav z namestitvijo za Microsoft DEFENDER ATP za Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
