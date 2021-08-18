---
title: Prepoznavanje dogodkov brisanja sporočil v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115664"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dnevniki nadzora za izbrisana e-poštna sporočila

Od januarja 2019 Microsoft privzeto vklanja pisanje dnevnika nadzora nabiralnika. Če želite pregledati dogodke sporočila za določenega uporabnika, morate ročno omogočiti dejanja brisanja za nadzor. Če je pisanje dnevnika nadzora nabiralnika že omogočeno za vašo organizacijo ali za določenega uporabnika, upoštevajte spodnja navodila.

1. Prijavite se v središče [za Microsoft 365 s predpisi](https://protection.office.com/)

2. Kliknite **Iskanje in raziskovanje in** izberite Iskanje v **dnevniku nadzora.**

3. Izberite datumski obseg v **poljih Začetni datum** in **Končni** datum. Določite uporabniško ime za uporabnika, ki ga želite raziskati (uporabnik, ki je izbrisal elemente). V polju **Dejavnosti** izberite Izbrisana sporočila **iz mape Izbrisano** in Premaknjena sporočila v mapo **Izbrisano.**

4. Kliknite **Iskanje.**

Med rezultati izberite zapis nadzora. V oknu s podrobnostmi kliknite **Več informacij.** Dodatne informacije o izbrisanem elementu (na primer vrstica z zadevo in mesto elementa, ko je bil izbrisan) so prikazane v polju **AffectedItems.** Lastnost **ClientInfoString** bo pokazala, če se je brisanje zgodilo v Outlook, Outlook v spletu (prej imenovani Outlook Web App) ali kateri koli drugi napravi.

Če želite več informacij, glejte [Določanje, kdo je nastavil posredovanje e-pošte za nabiralnik.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Opomba:** Izbrisanih elementov ne morete pridobiti s funkcijo dnevnika nadzora. Če želite izbrisana sporočila pridobiti Outlook v spletu programu, glejte [Obnovitev izbrisanih elementov Outlook programu Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
