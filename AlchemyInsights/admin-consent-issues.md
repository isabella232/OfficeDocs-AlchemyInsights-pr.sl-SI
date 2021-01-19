---
title: Težave s soglasjem skrbnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901512"
---
# <a name="admin-consent-issues"></a>Težave s soglasjem skrbnika

1. Omogočite [potek dela](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) skrbnika, če želite uporabnikom omogočiti, da zahtevajo skrbniško odobritev neposredno na zaslonu soglasja.

1. Če vi ali uporabniki aplikacije vidijo nepričakovane napake med postopkom odobritve, si oglejte ta članek navodila za odpravljanje težav: [Nepričakovana napaka pri izvajanju dovoljenja za program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Več informacij o [soglasju skrbnika na platformi Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kako deluje [poziv za privolitev](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) in kako [ovrednotiti zahtevo za odobritev skrbnika za celotno najemnika](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Programi, ki se integrirajo s platformo Microsoft Identity, spremljajo model avtorizacije, ki uporabnikom in skrbnikom omogoča nadzor nad tem, kako je mogoče dostopati do podatkov. Izvajanje modela za avtorizacijo je bilo posodobljeno na končni točki Microsoftovega izhodišča za identiteto in spremeni, kako mora program delovati z Microsoftovo platformo Identity. Če želite pregled tega modela odobritve, vključno s obsegi, dovoljenji in soglasjem, si oglejte [dovoljenja in soglasje v končni točki za Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .