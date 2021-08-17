---
title: Obračunavanje za rezerviran nakup primerka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104036"
---
# <a name="billing-for-reserved-instance-purchase"></a>Obračunavanje za rezerviran nakup primerka

Rezerviran primerek nakupa se zaračuna na način plačila, povezan z naročnino, ki jo izberete ob nakupu. Vrsta naročnine mora biti pogodba za podjetja (številka ponudbe: MS-AZR-0017P), Pay-As-You-Go (številka ponudbe: MS-AZR-0003P), Microsoftova pogodba o strankah ali CSP.

- Za naročnino podjetja so stroški obračunani iz zneska za denarne obveznosti včlanitve ali obračunanega kot prezapadli.
- Za naročnino na storitev Pay-As-You-Go so stroški zaračunani s kreditno kartico ali načinom plačila z računom v naročnini.

**Preklic rezervacije**

- **Samopostrežba:** rezervirani primerek lahko prekinete ali zamenjate sami s pomočjo [portala Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izberite rezervacijo in kliknite povračilo ali zamenjavo. Upoštevajte, da morate imeti lastniški dostop do naročila rezervacije za zamenjavo ali vračilo kupnine. Dostop samo do rezervacije vam ne bo omogočil vračila kupnine ali zamenjave. Prosite lastnika naročila rezervacije, da vam omogoči lastniški dostop do naročila rezervacije
- **Pravilnik o izmenjavi:** rezervacijo lahko zamenjate za drugo rezervacijo iste vrste – za zamenjavo rezervacije **ni predvidenih nobenih kazni**. Skupna obveznost z novo rezervacijo mora biti večja od vsote vračila zamenjane rezervacije in prihodnjih mesečnih plačil (če je primerno)
- **Politika vračila:** Vsota vračila in preklicana prihodnja plačila ne smejo preseči 50.000 USD v 12-mesečnem tekočem oknu. Trenutno **ne zaračunavamo nobene kazni** za vračila, lahko pa jo zaračunamo za prihodnja vračila

**Izjeme:** Možnost samopostrežne izmenjave in preklica ni na voljo strankam ameriškega vladnega poslovnega sporazuma

- Podpora za **API / PS / CLI** ni na voljo za preklic in povračila [ Samopostrežne menjave in vračila za rezervacije Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Možnost samopostrežne izmenjave in preklica ni na voljo strankam ameriškega vladnega poslovnega sporazuma. Podprte so druge vrste vladnih naročnin, vključno s Pay-As-You-Go in CSP

Več informacij: [Kako so obdelane transakcije vračila](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) in zamenjave Več informacij: Exchange in [pravilniki](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) za vračilo drugih vprašanj: [Obiščite rezervirane primerke dokumentov](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamenjajte obstoječi rezervirani primerek (samopostrežno)**

Rezervacijo lahko zamenjate za drugo rezervacijo iste vrste. Rezervacijo lahko vrnete, tudi do 50.000 USD na leto, če je ne potrebujete več. Možnost samopostrežne izmenjave in preklica ni na voljo strankam ameriškega vladnega poslovnega sporazuma. Podprte so druge vrste vladnih naročnin, vključno s Pay-As-You-Go in CSP. Morate imeti lastniški dostop do naročila rezervacije za zamenjavo ali vračilo kupnine obstoječe rezervacije.

Naslednji koraki vas bodo vodili skozi postopek za dokončanje transakcije

1.Prijavite se v portal [Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Izberite rezervacije, ki jih želite vračila kupnine, **in kliknite Exchange** 2.Izberite izdelek na VM, ki ga želite kupiti, in vnesite količino. Prepričajte se, da je skupna vrednost novega nakupa večja od skupne vrednosti vračanja, določite [pravo velikost pred nakupom.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Preglejte in dokončajte transakcijo

**Povračilo stroškov za rezervirani primerek**

Če želite povrniti rezervacijo, pojdite na **Podrobnosti o rezervaciji** in kliknite **Vračilo**

**Sorazmerno povračilo:**

**Pro primerov najmanjših zahtev za vračilo** in zamenjavo Primer rezervacije v vnaprej sesu:

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

**Računa za zadnje obdobje obračunavanja ni mogoče videti**

Nekateri možni razlogi, zakaj ne vidite računa:

- Za naročnino imate mesečni znesek dobropisa, ki ga niste presegli ali pa imate brezplačen preskus. Račun je ustvarjen le, če ste dolžni denar
- Čez manj kot 30 dni od dneva, ko ste se naročili na Azure
- Račun še ni ustvarjen. Počakajte do konca obračunskega obdobja
- Če niste skrbnik računa, morda za vas ne bodo na voljo starejši računi

**Prenesite račun s portala Azure (.pdf)**

- Izberite naročnino na strani [»Naročnine«](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) v portalu Azure kot [uporabnik z dostopom do računov](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Select **Invoices**
- Če si želite ogledati kopijo računa v obliki zapisa PDF, kliknite **Prenesi račun**. Če je navedeno **Ni na voljo**, si oglejte razdelek [Zakaj ne vidim računa za zadnje obdobje obračunavanja?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).

**Prejemanje računa po e-pošti (.pdf)**

- Izberite naročnino na [strani Naročnine.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Kliknite **»Računi« in** nato »Pošlji moj račun po e-pošti«
- Kliknite **privolitev v sodelovanje in** sprejmite pogoje. Za vsako naročnino morate privolti v sodelovanje v svoji

Opomba: Če po korakih ne dobite e-poštnega sporočila, preverite, ali je vaš e-poštni naslov pravilen v nastavitvah [komunikacije v profilu.](https://account.windowsazure.com/profile)

**Prenos podatkov o uporabi s portala Azure**

- Vpišite se v [središče računa Azure](https://account.windowsazure.com/Subscriptions) kot skrbnik [računa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Izberite naročnino, za katero želite informacije o računu in uporabi
- Izberite **»Zgodovina obračunavanja«**
- Izberite **Prikaži trenutno izjavo,** da si ogledate oceno stroškov v času, ko je bila ustvarjena ocena.
- Izberite **Prenos uporabe,** da prenesete podatke o dnevni uporabi kot datoteko CSV. Če sta na voljo dve različici, prenesite različico 2

Druga vprašanja: [Obiščite dokumente o rezerviranem primerku](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Priporočeni dokumenti**

- [Osnove obračunavanja](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje, kako je uporabljen popust rezerviranih primerkov](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos ali ogled računa za obračun za Azure in podatkov o dnevni uporabi](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje, kako je uporabljen popust rezerviranih primerkov](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervirane uporabe primerka za vašo naročnino na storitev Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervirane uporabe primerka za včlanitev podjetja](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows programske opreme niso vključeni v rezerviranih primerkov](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervirani primerki v programu Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)