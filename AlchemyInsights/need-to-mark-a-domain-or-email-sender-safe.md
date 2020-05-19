---
title: Potreba označiti domeno ali e-poštni pošiljatelj varno?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281187"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potreba označiti domeno ali e-poštni pošiljatelj varno?

- Uporaba **varnih seznamov pošiljateljev ni priporočljiva** , saj odpira vašo organizacijo v spam, Phish, in prevara napadov.
- Če pa obstaja poslovna zahteva, **priporočamo** , da za to uporabite **[pravila za pretok pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Naše smernice zagotavljajo avtentikacijo pošiljatelja (preveri, ali je domena pošiljateljica neponarejena). **Opomba**: ne priporočamo upravljanja lažnih pozitivnih rezultatov z uporabo varnih seznamov pošiljateljev, ker lahko izjeme pri filtriranju neželene pošte odprejo vašo organizacijo z varnostnimi napadi. Če uporabniki prejmejo sporočila, ki so nepravilno označena kot vsiljena ali neželena e-pošta, prosimo, **[prijavite sporočila in datoteke Microsoftu](https://protection.office.com/reportsubmission)**.
- Varen oddajnik v razgled, omogučiti oddajnik zapisati v seznam, ali omogučiti področje zapisati v seznam v smešen-spam policija **should obstati izogibati se** zato ker oddajnik bypass vsi spam, prevara, ter Phish varstvo, ter oddajnik AUTHENTICATION (SPF, DKIM, dMarc). Ta metoda se najbolje uporablja samo za začasno testiranje.
