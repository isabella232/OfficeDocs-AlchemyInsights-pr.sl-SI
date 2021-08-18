---
title: Odpravljanje težav z namestitvijo storitve MDATP v računalniku Mac
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091080"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Odpravljanje težav z namestitvijo storitve MDATP v računalniku Mac

Če ročna namestitev ne uspe, **se na** strani s povzetkom čarovnika za namestitev prikaže to sporočilo o napaki:

»Med namestitvijo je prišlo do napake. Namestitveni program je naletel na napako, zaradi katere namestitev ni uspela. Za pomoč se obrnite na izdelovalca programske opreme.«

Pri uvedbah programa MDM je na strani prikazano splošno napako pri namestitvi.

Čeprav končnim uporabnikom ne prikažemo točnih napak, dnevnik hranimo z napredkom namestitve v **/Library/Logs/Microsoft/mdatp/install.log.** Tej dnevniški datoteki je pripna vsaka namestitvena seja. Če želite izhod samo zadnje namestitvene seje, uporabite `sed` .

Če želite izvedeti več, glejte [Odpravljanje težav z namestitvijo za Microsoft Defender ATP za Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
