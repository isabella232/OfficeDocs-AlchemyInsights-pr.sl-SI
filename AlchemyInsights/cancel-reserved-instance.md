---
title: Preklic rezervacije
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807989"
---
# <a name="cancelling-reservation"></a>Preklic rezervacije

- **Samopostrežna storitev:** V storitvi [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)lahko prekličete ali zamenjate rezerviran primerek. Izberite rezervacijo in kliknite povračilo ali Exchange. Upoštevajte, da morate imeti lastnik dostop do naročila za rezervacijo za zamenjavo ali povračilo. Dostop le do rezervacije vam ne dovoli nadaljevati s povračilom ali zamenjavo. Prosite lastnika naročila za rezervacijo, da vam omogoči lastniku dostop do vrstnega reda rezervacij
- **Pravilnik za Exchange:** Rezervacijo lahko zamenjate za drugo rezervacijo iste vrste – pri izmenjavi rezervacij ni **kazni** . Skupna zaveza z novim rezervacijo bi morala biti večja od vsote zneska nadomestila, ki je bila izmenjana rezervacija, in prihodnjih mesečnih plačil (po potrebi)
- **Pravilnik o nadomestilu:** Vsota nadomestila in preklicana prihodnja plačila ne morejo presegati $50.000 USD v 12-mesečnem voznem oknu. **Trenutno ne zaračunavamo nobene kazni** za nadomestila, vendar bi jo lahko zaračunali na prihodnja nadomestila  
    **Izjeme:** Samopostrežna storitev Exchange in preklic zmogljivosti nista na voljo za stranke, ki so v podjetju ZDA
- Podpora **API/PS/CLI** ni na voljo za preklic in povračilo [samopostrežnih izmenjav in nadomestil za rezervacije Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samopostrežna storitev Exchange in preklic zmožnosti nista na voljo za stranke, ki so v podjetju ZDA. Druge vrste naročnine na AMERIŠKO vlado, vključno s plačili-as-you-go in CSP, so podprte

Več informacij: [Kako se obdelujejo vračanje in menjava transakcij](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Več informacij: [Pravilniki o izmenjavi in nadomestilih](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Druga vprašanja: [obiščite rezervirane vzorčne dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamenjava obstoječega rezerviranega primerka (samopostrežna storitev)**

Rezervacijo lahko zamenjate za drugo rezervacijo iste vrste. Rezervacijo lahko povrnete tudi do $50.000 USD na leto, če ga ne potrebujete več. Samopostrežna storitev Exchange in preklic zmožnosti nista na voljo za stranke, ki so v podjetju ZDA. Podprte so tudi druge vrste naročnine na AMERIŠKO vlado, vključno s plačili-as-you-go in CSP. Če želite zamenjati ali povrniti obstoječo rezervacijo, morate imeti lastnik dostop do naročila za rezervacijo.

Navodila za dokončanje transakcije se bodo prikazala v teh navodilih

1. Prijavite se v [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izberite rezervacije, ki jih želite povrniti, in kliknite **Exchange**
2. Izberite izdelek VM, ki ga želite kupiti, in vnesite količino. Prepričajte se, da je nova skupna vsota nakupov večja od skupne vsote, ki [določa pravo velikost pred nakupom](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Preglejte in dokončajte transakcijo

**Povračilo za rezerviran primer**

Če želite povrniti rezervacijo, pojdite na **podrobnosti rezervacije** in kliknite **vračilo** .

**Proocenjeno nadomestilo:**

**Primeri Pro-obroka in minimalne zahteve za povračilo in zamenjavo**  
Primer vnaprejšnje rezervacije:

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

**Priporočeni dokumenti**

- [Kako se obdelujejo vračanje in menjava transakcij](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Pravilniki o izmenjavi in nadomestilih](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)