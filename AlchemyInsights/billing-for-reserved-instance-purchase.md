---
title: Obračunavanje za rezervirani primerek nakupa
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820338"
---
# <a name="billing-for-reserved-instance-purchase"></a>Obračunavanje za rezervirani primerek nakupa

Rezervirani primerek nakupa se zaračuna na način plačila, povezan z naročnino, ki jo izberete ob nakupu. Vrsta naročnine mora biti pogodba podjetja (številka ponudbe: MS-AZR-0017P), Pay-As-You-Go (številka ponudbe: MS-AZR-0003P), Microsoftova pogodba za stranke ali CSP.

- Za naročnino podjetja so zaračunani stroški iz denarnih obveznosti v včlanitve ali zaračunani kot prekomerno
- Za naročnino na storitev Pay-As-You-Go so stroški zaračunani načinu plačila s kreditno kartico ali z računom v naročnini

**Preklic rezervacije**

- **Samopostrežna storitev:** Rezerviran primerek lahko prekličete ali zamenjate sami s [portalom Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izberite rezervacijo in kliknite vračilo kupnine ali zamenjavo. Če želite zamenjavo ali vračilo kupnine, morate imeti dostop lastnika v naročilu rezervacije. Dostop le do rezervacije vam ne omogoča vračila denarja ali zamenjave. Prosite lastnika naročila rezervacije, da vam lastniku da dostop do naročila rezervacije
- **Pravilnik strežnika Exchange:** Če želite, lahko rezervacijo za drugo vrsto  rezervacije zamenjate brez rezervacij. Skupna obveznost z novo rezervacijo mora biti večja od vsote vračila kupnine iz zamenjane rezervacije in prihodnjih mesečnih obrokov (če so na voljo)
- **Pravilnik za vračilo kupnine:** Vsota vračila in preklicana prihodnja plačila v 12-mesečnem oknu ne sme presegati 50.000 USD. Trenutno ne **bremenjumo nobene stroške za vračila** kupnine, vendar bi ga lahko zaračunali na prihodnjih vračilih

**Izjeme:** Samopostrežna zamenjava in preklic možnosti ni na voljo za stranke sporazuma US Government Enterprise Agreement

- **Podpora za API/PS/CLI** ni na voljo za preklic in vračila denarja Samopostrežna borza [in vračila denarja za storitve Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samopostrežna zamenjava in preklic možnosti ni na voljo za stranke sporazuma US Government Enterprise Agreement. Podprte so tudi druge vrste naročnin zda Government, vključno s pay-as-you-go in CSP.

Več informacij: [Kako so obdelane transakcije vračila](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) in zamenjave Več informacij: [Pravilniki](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) za Exchange in vračilo denarja Druga vprašanja: [Obisk rezerviranih primerkov dokumentov](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamenjava obstoječega rezerviranega primerka (samopostrežna storitev)**

Rezervacijo za drugo rezervacijo enake vrste lahko zamenjate. Če je ne potrebujete več, lahko tudi plačate rezervacijo v višini 50.000 USD na leto, če je ne potrebujete več. Samopostrežna zamenjava in preklic možnosti ni na voljo za stranke sporazuma US Government Enterprise Agreement. Podprte so tudi druge vrste naročnin zda Government, vključno s pay-as-you-go in CSP. Če želite obstoječo rezervacijo zamenjati ali vračila kupnine, morate imeti dostop lastnika v naročilu rezervacije.

V spodnjih korakih boste našli navodila za dokončanje transakcije.

1.Prijavite se v portal [Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Izberite rezervacije, ki jih želite povrniti, in kliknite **Exchange** 2.Izberite izdelek na VM, ki ga želite kupiti, in vnesite količino. Prepričajte se, da je skupna vrednost novega nakupa večja od skupne vrednosti vračanja, določite [pravo velikost pred nakupom.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Preglejte in dokončajte transakcijo

**Vračilo kupnine za rezervirani primerek**

Če želite vrniti rezervacijo, pojdite v podrobnosti **rezervacije in** kliknite »Vračilo **kupnine«**

**Povračilo za povračilo:**

**Primeri promocijske in minimalne zahteve za vračilo denarja in zamenjavo** Primer rezervacije v vnaprej sesu:

- Kupite enoletno obdobje RI za 120 $ 1. januarja
- 7. aprila želite vrniti kupnino ali je ta rezervacija zamenjana
- Ker je rezervacija v živo 97 dni, boste dobili (1–97/365) * 120 $ nazaj. (to je 88,1 USD). O vračilih kupnine trenutno ni na voljo nobeno vračilo kupnine
- Če si izmenjate, bi moral vaš novi nakup biti večji od 88,1 $
- O vračilih kupnine trenutno ni na voljo

**Primer rezervacije načrta obračunavanja:**

- Kupite enoletno obdobje RI za 10 USD na mesec
- 7. aprila želite vrniti kupnino ali je ta rezervacija zamenjana
- Ker je bilo zadnje plačilo 7 dni, boste dobili (1-7/31) * 10 USD nazaj. (to je 7,74 $)
- Bodoča preklicana plačila so 80 $. O vračilih kupnine trenutno ni na voljo nobeno vračilo kupnine
- Ta preklic prekliče naročnino na znesek 87,74 USD, če ste omejitev vračila kupnine za 50.000 $
- Če izmenjavo podatkov, mora biti skupna vrednost novega nakupa večja od 87,74 $.

**Računa za zadnje obdobje obračunavanja ni mogoče videti**

Nekateri možni razlogi, zakaj ne vidite računa:

- Za naročnino imate mesečni znesek dobropisa, ki ga niste presegli ali pa imate brezplačen preskus. Račun je ustvarjen le, če ste dolžni denar
- Čez manj kot 30 dni od dneva, ko ste se naročili na Azure
- Račun še ni ustvarjen. Počakajte do konca obračunskega obdobja
- Če niste skrbnik računa, morda za vas ne bodo na voljo starejši računi

**Prenesite račun s portala Azure (.pdf)**

- Izberite naročnino na strani [»Naročnine«](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) v portalu Azure kot [uporabnik z dostopom do računov](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Select **Invoices**
- Kliknite **Prenesi račun,** da si ogledate kopijo računa PDF. Če piše **Ni na** voljo, glejte Zakaj ne vidim računa za zadnje obdobje [obračunavanja?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

Druga vprašanja: [Obiščite rezervirane primerke dokumentov](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Priporočeni dokumenti**

- [Osnove obračunavanja](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje, kako je uporabljen popust rezerviranih primerkov](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos ali ogled računa za obračun za Azure in podatkov o dnevni uporabi](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje, kako je uporabljen popust rezerviranih primerkov](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervirane uporabe primerka za vašo naročnino na storitev Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervirane uporabe primerka za včlanitev podjetja](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stroški programske opreme Windows niso vključeni v rezerviranih primerkov](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervirani primerki v programu Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)