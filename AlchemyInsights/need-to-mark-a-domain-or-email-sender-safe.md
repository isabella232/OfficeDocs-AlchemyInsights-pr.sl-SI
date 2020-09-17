---
title: Ali želite označiti varno domeno ali pošiljatelja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803261"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Ali želite označiti varno domeno ali pošiljatelja e-pošte?

- Uporaba **seznamov varnih pošiljateljev ni priporočljiva** , saj vaša organizacija odpre vašo organizacijo za neželeno pošto, Phish in lažne napade.
- Če pa obstaja poslovna zahteva, **priporočamo** , da za to uporabite **[pravila za tok pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Naše vodilo zagotavlja preverjanje pristnosti pošiljatelja (preveri, ali je domena za pošiljanje lažna). **Opomba**: ne priporočamo, da na seznamih varnih pošiljateljev uporabite lažne pozitivne izraze, ker lahko izjeme do filtriranja neželene pošte odprejo vašo organizacijo na varnostne napade. Če vaši uporabniki prejmejo sporočila nepravilno označena kot neželena ali neželena e-pošta, pošljite **[Microsoftu sporočila o sporočilih in datotekah](https://protection.office.com/reportsubmission)**.
- Varni pošiljatelji v Outlooku, dovoljen seznam pošiljatelja ali dovoljen seznam domen v pravilnikih za preprečevanje neželene pošte se **morajo izogibati** , ker pošiljatelji zaobidejo vse neželene pošte, spoof in Phish zaščito ter preverjanje pristnosti pošiljatelja (SPF, DKIM, DMARC). Ta način je najbolje uporabiti le za začasno testiranje.
