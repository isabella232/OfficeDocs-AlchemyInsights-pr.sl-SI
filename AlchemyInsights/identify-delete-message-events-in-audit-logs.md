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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696529"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Dnevniki nadzora za izbrisana e-poštna sporočila

Z začetkom januarja 2019 se Microsoft samodejno vklopi v dnevnik nadzora nabiralnika. V nasprotnem primeru za pregled brisanja dogodkov sporočila za določenega uporabnika morate ročno omogočiti dejanja brisanja za nadzor. Če je pisanje dnevnika nadzora nabiralnika že omogočeno za vašo organizacijo ali za določenega uporabnika, upoštevajte spodnja navodila.

1. Prijavite se v [središče za varnost & skladnost s predpisi Microsoft 365](https://protection.office.com/)

2. Kliknite **iskanje in preiskovanje** in izberite **iskanje dnevnika nadzora**.

3. Izberite datumski obseg v poljih **Začetni datum** in **končni datum** . Določite uporabniško ime za uporabnika, ki ga želite raziskati (uporabnik, ki je izbrisal elemente). V polju **dejavnosti** izberite **izbrisana sporočila iz mape» Izbrisano «** in **premaknjena sporočila v mapo» Izbrisano «**.

4. Kliknite **Išči**.

V rezultatih Izberite zapis nadzora. V razdelku podrobnosti flyout kliknite **več informacij**. Dodatne informacije o izbrisanem elementu (na primer vrstica z zadevo in lokacija elementa, ko je bila izbrisana) je prikazana v polju» **AffectedItems** «. Lastnost **ClientInfoString** se prikaže, če je prišlo do brisanja v Outlooku, Outlooku v spletu (prej znan kot Outlook Web App) ali kateri koli drugi napravi.

Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Opomba**: izbrisanih elementov ne morete pridobiti s funkcijo dnevnika nadzora. Če želite pridobiti izbrisana sporočila v Outlooku v spletu, [si oglejte obnovitev izbrisanih elementov v programu Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
