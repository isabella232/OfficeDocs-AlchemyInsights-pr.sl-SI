---
title: Preklic rezervacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931249"
---
# <a name="cancelling-reservation"></a>Preklic rezervacije

- **Samopostrežba:** rezervirani primerek lahko prekinete ali zamenjate sami s pomočjo [portala Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izberite rezervacijo in kliknite povračilo ali zamenjavo. Upoštevajte, da morate imeti lastniški dostop do naročila rezervacije za zamenjavo ali vračilo kupnine. Dostop samo do rezervacije vam ne bo omogočil vračila kupnine ali zamenjave. Prosite lastnika naročila rezervacije, da vam omogoči lastniški dostop do naročila rezervacije
- **Pravilnik o izmenjavi:** rezervacijo lahko zamenjate za drugo rezervacijo iste vrste – za zamenjavo rezervacije **ni predvidenih nobenih kazni**. Skupna obveznost z novo rezervacijo mora biti večja od vsote vračila zamenjane rezervacije in prihodnjih mesečnih plačil (če je primerno)
- **Politika vračila:** Vsota vračila in preklicana prihodnja plačila ne smejo preseči 50.000 USD v 12-mesečnem tekočem oknu. Trenutno **ne zaračunavamo nobene kazni** za vračila, lahko pa jo zaračunamo za prihodnja vračila  
    **Izjeme:** Možnost samopostrežne izmenjave in preklica ni na voljo strankam ameriškega vladnega poslovnega sporazuma
- Podpora za **API / PS / CLI** ni na voljo za preklic in povračila [ Samopostrežne menjave in vračila za rezervacije Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Možnost samopostrežne izmenjave in preklica ni na voljo strankam ameriškega vladnega poslovnega sporazuma. Podprte so druge vrste vladnih naročnin, vključno s Pay-As-You-Go in CSP

Več informacij : [Kako se obdelujejo transakcije vračanja in menjave](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Več informacij : [Pravilniki o zamenjavi in ​​vračilu kupnine](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Druga vprašanja: [Obiščite dokumente o rezerviranem primerku](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamenjajte obstoječi rezervirani primerek (samopostrežno)**

Rezervacijo lahko zamenjate za drugo rezervacijo iste vrste. Rezervacijo lahko vrnete, tudi do 50.000 USD na leto, če je ne potrebujete več. Možnost samopostrežne izmenjave in preklica ni na voljo strankam ameriškega vladnega poslovnega sporazuma. Podprte so druge vrste vladnih naročnin, vključno s Pay-As-You-Go in CSP. Morate imeti lastniški dostop do naročila rezervacije za zamenjavo ali vračilo kupnine obstoječe rezervacije.

Naslednji koraki vas bodo vodili skozi postopek za dokončanje transakcije

1. Prijavite se v vaš[portal Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izberite rezervacije, ki jih želite vrniti, in kliknite **Zamenjava**
2. Izberite izdelek VM, ki ga želite kupiti, in vnesite količino. Prepričajte se, da je skupna vrednost novega nakupa večja od skupne vrednosti vrnitve [Pred nakupom določite pravo velikost](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Predogled in dokončanje transakcije

**Povračilo stroškov za rezervirani primerek**

Če želite povrniti rezervacijo, pojdite na **Podrobnosti o rezervaciji** in kliknite **Vračilo**

**Sorazmerno povračilo:**

**Sorazmerno povračilo in primeri minimalnih zahtev za vračilo in zamenjavo kupnine**  
Primer predhodne rezervacije:

- 1. januarja kupite enoletni RP za 120 USD
- 7. aprila želite to rezervacijo povrniti ali zamenjati
- Ker je rezervacija aktivna že 97 dni, boste dobili povrnjenih (1-97/365) * 120 USD. (tj. 88,1 USD). Trenutno ni nobene predvidene kazni glede povračila kupnine
- Če opravite zamenjavo, mora biti vaš novi nakup višji od 88,1 USD
- Trenutno ni nobene predvidene kazni glede povračila kupnine

**Primer rezervacije načrta za obračunavanje:**

- Kupite enoletni RP za 10 USD mesečno
- 7. aprila želite to rezervacijo povrniti ali zamenjati
- Ker je bilo zadnje plačilo opravljeno pred 7 dnevi, boste dobili povrnjenih (1-7/31) * 10 USD. (tj. 7,74 USD)
- Prihodnja preklicana plačila bodo znašala 80 USD. Trenutno ni nobene predvidene kazni glede povračila kupnine
- Ta preklic bo od vaše omejitve vračila v višini 50.000 USD odštel 87,74 USD
- Če opravite zamenjavo, mora biti skupna vrednost vašega novega nakupa višja od 87,74 USD

**Priporočeni dokumenti**

- [Kako se obdelujejo transakcije vračanja in menjave](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Pravilniki o zamenjavi in ​​vračilu kupnine](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)