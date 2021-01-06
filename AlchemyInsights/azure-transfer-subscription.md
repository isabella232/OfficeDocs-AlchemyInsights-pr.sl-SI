---
title: Prenos lastništva za obračunavanje Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755563"
---
# <a name="transfer-azure-billing-ownership"></a>Prenos lastništva za obračunavanje Azure

Vpišite se v [Azure portal](https://portal.azure.com/) kot skrbnik računa za obračunavanje z naročnino, ki jo želite prenesti. Če niste prepričani, ali ste skrbnik ali če morate ugotoviti, kdo je, glejte [določanje skrbniškega računa za obračunavanje](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Poiščite _Upravljanje stroškov + obračunavanje_.
1. Izberite **naročnine** v levem podoknu. Glede na dostop boste morda morali izbrati obseg obračunavanja in nato **naročnine** ali **naročnine Azure**.
1. Za naročnino, ki jo želite prenesti, izberite **Prenesi lastništvo obračunavanja** .
1. Vnesite e-poštni naslov uporabnika, ki je skrbnik za obračunavanje računa, ki bo nov lastnik naročnine, nato pa izberite **pošljite zahtevo za prenos**.
1. Uporabnik prejme e-poštno sporočilo z navodili za pregled vaše zahteve za prenos. Če želite odobriti zahtevo za prenos, uporabnik izbere povezavo v e-poštnem sporočilu in sledi navodilom.

Če želite, da je lastništvo naročnine na uporabniški račun v drugem najemniku storitve Azure AD, morate vse [nadzor dostopa, ki temelji na vlogi,](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) naloge za upravljanje virov v naročnini, trajno odstraniti. Za upravljanje virov v naročnini bo imel dostop le nov lastnik. Če želite več informacij o tem, kako spremenite imenik za naročnino, glejte [prenašanje naročnine na uporabnika v drugem najemniku storitve Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Pomembno vplivanje na vaše račune**_: Če ste za naročnino na Azure prenesli lastništvo nad obračunom, bodo vaše cene proovrednotene. Do računov boste lahko dostopali tako, da bodo na voljo:  

1. Izberite naročnino na strani [naročnine, ki](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) v portalu Azure kot [uporabnik z dostopom do računov](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), nato pa izberite **računi**.
1. Če si želite ogledati kopijo računa v obliki zapisa PDF, kliknite **Prenesi račun** . Če je navedeno, da _ni na voljo_, glejte [zakaj ne vidim računa za zadnje obdobje obračunavanja?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Dnevno uporabo lahko prikažete tudi tako, da kliknete **obdobje obračunavanja** za pridobitev datoteke PDF, ki je na svojem računu, in kopijo vaše podrobne aplikacije za dnevno uporabo (. CSV). Če želite več informacij, glejte [dobite podatke o računu in uporabi](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Priporočeni dokumenti**

- [Prenos lastništva naročnine na storitev Azure v drug račun](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Če želite prenesti lastništvo obračunavanja za naročnino na Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prenos Visual Studio, Microsoft partner Network (MPN) in Pay as you go dev/preskusne naročnine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Pogosta vprašanja o prenosu lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Odpravljanje težav s prenosom lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
