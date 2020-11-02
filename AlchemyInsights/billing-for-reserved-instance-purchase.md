---
title: Obračunavanje za rezervirani primer nakupa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823170"
---
# <a name="billing-for-reserved-instance-purchase"></a>Obračunavanje za rezervirani primer nakupa

Naročnina na primer je plačana načinu plačila, ki je vezan na naročnino, ki ste jo izbrali ob času nakupa. Vrsta naročnine mora biti pogodba podjetja (ponudba številka: MS-AZR-0017P), Pay-as-you-go (ponudba številka: MS-AZR-0003P), Microsoft Customer pogodbe ali CSP.

- Za naročnino na podjetje se stroški odštejejo od zneska denarne obveznosti za vpis ali pa so zaračunani kot preveliki
- Za naročnino na plačilo – as-you-go se stroški zaračunajo na kreditno kartico ali način plačila računa na naročnino

**Preklic rezervacije**

- **Samopostrežna storitev:** V storitvi [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)lahko prekličete ali zamenjate rezerviran primerek. Izberite rezervacijo in kliknite povračilo ali Exchange. Upoštevajte, da morate imeti lastnik dostop do naročila za rezervacijo za zamenjavo ali povračilo. Dostop le do rezervacije vam ne dovoli nadaljevati s povračilom ali zamenjavo. Prosite lastnika naročila za rezervacijo, da vam omogoči lastniku dostop do vrstnega reda rezervacij
- **Pravilnik za Exchange:** Rezervacijo lahko zamenjate za drugo rezervacijo iste vrste – pri izmenjavi rezervacij ni **kazni** . Skupna zaveza z novim rezervacijo bi morala biti večja od vsote zneska nadomestila, ki je bila izmenjana rezervacija, in prihodnjih mesečnih plačil (po potrebi)
- **Pravilnik o nadomestilu:** Vsota nadomestila in preklicana prihodnja plačila ne morejo presegati $50.000 USD v 12-mesečnem voznem oknu. **Trenutno ne zaračunavamo nobene kazni** za nadomestila, vendar bi jo lahko zaračunali na prihodnja nadomestila

**Izjeme:** Samopostrežna storitev Exchange in preklic zmogljivosti nista na voljo za stranke, ki so v podjetju ZDA

- Podpora **API/PS/CLI** ni na voljo za preklic in povračilo [samopostrežnih izmenjav in nadomestil za rezervacije Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samopostrežna storitev Exchange in preklic zmožnosti nista na voljo za stranke, ki so v podjetju ZDA. Druge vrste naročnine na AMERIŠKO vlado, vključno s plačili-as-you-go in CSP, so podprte

Več informacij: [Kako se lahko obdelajo Return in Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) , preberite več o tem: [Pravilniki za Exchange in nadomestila](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) druga vprašanja: [obiščite rezervirane vzorčne dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamenjava obstoječega rezerviranega primerka (samopostrežna storitev)**

Rezervacijo lahko zamenjate za drugo rezervacijo iste vrste. Rezervacijo lahko povrnete tudi do $50.000 USD na leto, če ga ne potrebujete več. Samopostrežna storitev Exchange in preklic zmožnosti nista na voljo za stranke, ki so v podjetju ZDA. Podprte so tudi druge vrste naročnine na AMERIŠKO vlado, vključno s plačili-as-you-go in CSP. Če želite zamenjati ali povrniti obstoječo rezervacijo, morate imeti lastnik dostop do naročila za rezervacijo.

Navodila za dokončanje transakcije se bodo prikazala v teh navodilih

1. Prijavite se v [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izberite rezervacije, ki jih želite povrniti, in kliknite **Exchange** 2. Izberite izdelek VM, ki ga želite kupiti, in vnesite količino. Prepričajte se, da je nova skupna vsota nakupov večja od skupne vsote, ki [določa pravo velikost pred nakupom](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. preglejte in dokončajte transakcijo

**Povračilo za rezerviran primer**

Če želite povrniti rezervacijo, pojdite na **podrobnosti rezervacije** in kliknite **vračilo** .

**Proocenjeno nadomestilo:**

**Primeri Pro-obroka in minimalne zahteve za povračilo in zamenjavo** Primer vnaprejšnje rezervacije:

- Kupite enoletno obdobje RI za $120 v januarju 1
- 7. april želite povrniti ali zamenjati rezervacijo
- Ker je rezervacija v živo za 97 dni, boste dobili (1-97/365) * $120 vrnil. (tj. $88,1). Trenutno ni na voljo nobena kazen za povračilo
- Če želite, da bo vaš novi nakup večji od $88,1
- Trenutno ni nobene kazni za nadomestila

**Primer rezervacije načrta obračunavanja:**

- Kupite enoletno obdobje RI za $10 na mesec
- 7. april želite povrniti ali zamenjati rezervacijo
- Od zadnjega plačila se je zgodilo 7 dni, boste dobili (1-7/31) * $10 vrnil. (tj. $7,74)
- Preklicana prihodnja plačila so $80. Trenutno ni na voljo nobena kazen za povračilo
- Ta preklic bo odštel $87,74 od vašega zneska $50.000 nadomestila
- Če je zamenjava, mora biti skupna vrednost novega nakupa večja od $87,74.

**Računa za zadnje obdobje obračunavanja ni mogoče videti**

Nekaj možnih razlogov, zakaj morda ne vidite računa:

- Imate mesečni znesek kredita z naročnino, ki je niste presegli ali pa imate brezplačno preskusno različico. Račun je ustvarjen le, ko dolgujete denar.
- To je manj kot 30 dni od dneva, ko ste naročeni na Azure
- Račun še ni ustvarjen. Počakaj do konca obdobja obračunavanja
- Če niste skrbnik računa, starejši računi morda ne bodo na voljo za vas

**Prenos računa iz portala Azure (. pdf)**

- [Na strani»](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) naročnine «na spletnem portalu Azure izberite svojo naročniško razmerje kot [uporabnik z dostopom do računov](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Izberite **računi**
- Kliknite **Prenesi račun** , če si želite ogledati kopijo računa PDF. Če je navedeno, da **ni na voljo** , glejte [zakaj ne vidim računa za zadnje obdobje obračunavanja?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Prejemanje računa v e-pošti (. pdf)**

- Izberite svojo naročnino [na strani naročnin](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Kliknite **računi** nato Pošlji e-pošto na moj račun
- Kliknite **opt** in Sprejmi pogoje. Za vsako naročnino, ki jo imate, boste morali izbrati

Opomba: Če po korakih ne dobite e-poštnega sporočila, se prepričajte, da je vaš e-poštni naslov pravilen v [nastavitvah komunikacije v profilu](https://account.windowsazure.com/profile) .

**Prenos podatkov o uporabi iz portala Azure**

- Vpišite se v [središče za račun Azure](https://account.windowsazure.com/Subscriptions) kot [skrbnik računa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Izberite naročnino, za katero želite, da so informacije o računu in uporabi
- Izberite **zgodovino obračunavanja**
- Izberite **Prikaži trenutno izjavo** , da si ogledate oceno stroškov v času, ko je bila ocena ustvarjena.
- Izberite **Prenesi uporabo** , da prenesete podatke dnevne uporabe kot datoteko CSV. Če vidite dve različici, ki sta na voljo, prenesite različico 2

Druga vprašanja: [obiščite rezervirane vzorčne dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Priporočeni dokumenti**

- [Osnove obračunavanja](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje načina uporabe rezerviranega primerka](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos ali ogled računa za obračun in dnevne uporabe podatkov v storitvi Azure](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje načina uporabe rezerviranega primerka](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje uporabe rezerviranih primerkov za naročnino na plačilo – as-you-go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje uporabe rezerviranih primerkov za včlanitev podjetja](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stroški programske opreme sistema Windows, ki niso vključeni v rezervirane primerke](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervirani primerki v programu partner centralnega ponudnika oblak rešitev (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)