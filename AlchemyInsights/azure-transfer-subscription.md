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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922170"
---
# <a name="transfer-azure-billing-ownership"></a>Prenos lastništva za obračunavanje Azure

Vpišite se v [portal Azure](https://portal.azure.com/) kot skrbnik računa obračunavanja, ki ima naročnino, ki jo želite prenesti. Če niste prepričani, ali ste skrbnik ali če želite ugotoviti, kdo je, glejte [določanje skrbnika obračunavanja računov](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Iskanje po **stroških upravljanja + obračunavanje**.
- V levem podoknu izberite **naročnine** . Odvisno od Accessa boste morda morali izbrati obseg obračunavanja **in nato naročnine** ali **Azure naročnine**.
- Izberite» **prenos lastništva računa** «za naročnino, ki jo želite prenesti
- Vnesite e-poštni naslov uporabnika, ki je skrbnik za obračunavanje računa, ki bo novi lastnik za naročnino, nato pa izberite **Pošlji zahtevo za prenos**
- Uporabnik dobi e-poštno sporočilo z navodili za pregled zahteve za prenos. Če želite odobriti zahtevo za prenos, uporabnik izbere povezavo v e-poštnem sporočilu in sledi navodilom.

**Opomba** : Če želite prenesti lastništvo nad naročnino na uporabniški račun v drugem najemniku storitve Azure ad, je treba trajno odstraniti vse naloge [nadzora dostopa, ki temeljijo na vlogi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)za upravljanje virov v naročnini. Le novi lastnik bo imel dostop do upravljanja virov v naročnini. Če želite več informacij, glejte [prenos naročnine na uporabnika v drugem najemniku storitve AZURE ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Priporočeni dokumenti**

- [Prenos lastništva naročnine na storitev Azure na drug račun](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [O prenosu lastništva obračunavanja za naročnino na Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prenos vizualnega studia, Microsoft partnerskega omrežja (MPN) in plačila po naročnini za dev/test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Pogosta vprašanja o prenosu lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Odpravljanje težav pri prenosu lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
