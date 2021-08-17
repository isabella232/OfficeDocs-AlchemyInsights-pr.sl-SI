---
title: Odpravljanje pogostih težav s programom Microsoft Defender za Office 365
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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898260"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Odpravljanje pogostih težav s programom Microsoft Defender za Office 365

Tukaj je nekaj rešitev za pogoste težave s programom Microsoft Defender za Office 365:

- **Zakasnitev sporočila:**

  Do zakasnitev pri dostavi e-pošte lahko Sef pregledovanje sporočil prilog. Če želite več informacij, [Sef nastavitev pravilnika o prilogah.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Poročilo vsebuje napačne pozitivne ali negativne rezultate:**

  Če želite več informacij, [glejte Poročanje sporočil in datotek Microsoftu.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Omogočanje Sef povezave:**

  1. V portalu Microsoft 365 Defender v razdelku Pravilniki sodelovanja med e-& in & pravilniki o grožnjah <https://security.microsoft.com/>  \>  \>  \> **za Sef povezavami** v **razdelku Pravilniki.**

     Če želite neposredno na **Sef Povezave,** uporabite <https://security.microsoft.com/safelinksv2> .

  2. Na **Sef povezave** izberite pravilnik tako, da kliknete ime pravilnika.
  3. V prikazanem oknu s podrobnostmi naredite nekaj od tega:
     - Če želite dodati nov pravilnik, izberite **+ Ustvari**. Zažene se čarovnik, ki vam bo pomagal določiti nastavitve pravilnika.
     - Če želite urediti obstoječi pravilnik, izberite pravilnik tako, da kliknete ime pravilnika. V prikazanem oknu s podrobnostmi izberite **Uredi** v razdelku **Nastavitve** zaščite.
  4. Na **strani Nastavitve zaščite** konfigurirajte te nastavitve:
     - Vklopite **možnost Izberite dejanje za neznane morebitne zlonamerne URL-je v sporočilih.**
     - Izberite **Uporabi varne povezave za sporočila, poslana znotraj organizacije.**

  Če želite več informacij, [glejte Nastavitev pravilnikov Sef za povezave v programu Microsoft Defender za Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
