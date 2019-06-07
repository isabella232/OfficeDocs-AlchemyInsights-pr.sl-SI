---
title: Prepoznavanje Izbriši sporočilo dogodkov v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755168"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dnevnikov za izbrisati email vest

Odhod v januarju 2019, Microsoft zavija na nabiralnik revizije prijavi privzeto. Drugače, pregled izbrisati sporočilo dogodkov za določenega uporabnika, boste morali ročno omogočiti dejanja delete za revidiranje. Če nabiralnik revizijo pisanje dnevnika je že omogočeno za organizacijo ali za določenega uporabnika, sledite spodnjim korakom.

1. Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/)

2. Kliknite **Išči ter preiskave** in izberite **Išči dnevnika nadzora**.

3. Izberite datumski obseg v polji **Začetni datum** in **končni datum** . Določite uporabniško ime uporabnika, ki jo želite raziskati (uporabnik, ki je izbrisano). Na področju **dejavnosti** , izberite **izbrisana sporočila iz mape Izbrisano** in **premaknjeno sporočila v mapo Izbrisano**.

4. Kliknite **Išči**.

V rezultate, izberite revizijski zapis. V pojavni meni podrobnosti, kliknite **Več informacij**. Dodatne informacije o izbrisanega elementa (na primer, zadevo in mesto elementa, ko je bila izbrisana) je prikazana v polju **AffectedItems** . Lastnost **ClientInfoString** prikaže, če izbris je prišlo v Outlooku, Outlook v spletu (prej znan kot Outlook Web App), ali katere koli druge naprave.

Če želite več informacij, glejte [določanje ki nastaviti e-pošte, posredovanje za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Opomba**: ne more pridobiti izbrisano funkcijo dnevnika nadzora. Če naložite izbrisana sporočila v Outlook v spletu, glejte [obnavljanje izbrisanih elementov v storitvi Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
