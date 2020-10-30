---
title: Podprte vrste naročnine
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807980"
---
# <a name="supported-subscription-types"></a>Podprte vrste naročnine

Če želite nadaljevati, si oglejte podprte vrste naročnine.

[Podprte vrste naročnine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prenos lastništva plačnika**

Portal Azure kot [skrbnik računa](https://ms.portal.azure.com/) za račun za obračunavanje, ki ima naročnino, ki jo želite prenesti

- Iskanje po **stroških upravljanja + obračunavanje** . V levem podoknu izberite **naročnine** . Odvisno od Accessa boste morda morali izbrati obseg obračunavanja **in nato naročnine** ali **Azure naročnine** .
- Izberite» prenos lastništva računa «za naročnino, ki jo želite prenesti
- Vnesite e-poštni naslov uporabnika, ki je skrbnik za obračunavanje računa, ki bo novi lastnik za naročnino, nato pa izberite **Pošlji zahtevo za prenos**
- Uporabnik dobi e-poštno sporočilo z navodili za pregled zahteve za prenos. Če želite odobriti zahtevo za prenos, uporabnik izbere povezavo v e-poštnem sporočilu in sledi navodilom.

Opomba: Če želite prenesti lastništvo nad naročnino na uporabniški račun v drugem najemniku storitve Azure AD, je treba trajno odstraniti vse naloge [nadzora dostopa, ki temeljijo na vlogi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje virov v naročnini. Le novi lastnik bo imel dostop do upravljanja virov v naročnini. Če želite več informacij, glejte [prenos naročnine na uporabnika v drugem najemniku storitve AZURE ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenos lastništva naročnine**

Naročnina za prenos lastništva za upravljanje virov v naročnini izgubi dostop. Če želite več informacij o dodajanju obstoječe naročnine najemniku, glejte [povezovanje ali dodajanje naročnine na Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenos naročnine z obstoječim neporavnanim zneskom iz trenutnega cikla obračunavanja v novem računu ne bo prenesen v nov plačilni instrument. Le informacije, ki so na voljo uporabnikom v novem računu, so stroški zadnjega meseca za vašo naročnino. Preostali del uporabe in zgodovina obračunov se ne prenesejo z naročnino.
- Naročnine na prenos lastništva poslovnih sporazumov (EA) je trenutno podprta le v portalu za podjetja s sporazumi
- Prenos kreditne usmerjenih naročnine, kot je Visual Studio, BizSpark, Microsoft partnersko omrežje za novega uporabnika zahteva, da ima Visual Studio/Microsoft partnersko omrežno licenco, da sprejme zahtevo za prenos
- Vsi viri, kot so navidezni stroji, diski in spletna mesta, so uspešno preneseni v nov račun. Na prenos naročnine prek najemnika lahko vplivajo ti viri:

**Domenske storitve Azure AD**

Trezorji Azure Key

- [Povezani uporabniki in zbirke podatkov SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) lahko vplivajo, še posebej, če stranka uporablja preverjanje pristnosti, povezane z imenikom Azure Active Directory.
- **Storitve programov** , konfigurirane z preverjanjem pristnosti imenika Azure Active Directory
- **Skupina za Visual Studio** Računi storitve, ki so priključeni na naročnine na Azure, lahko začasno izgubijo dostop, ko je povezava s povezavo Azure preklicana

**Priporočeni dokumenti**

Koraki po sprejetju lastništva plačnika:

- Če želite ohraniti lastništvo obračuna, vendar spremenite vrsto naročnine, glejte: [preklop naročnine na Azure na drugo ponudbo](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos vizualnega studia, Microsoft partnerskega omrežja (MPN) in plačila po naročnini za dev/test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos lastništva v naročnini na podjetja (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Pogosta vprašanja o prenosu lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Odpravljanje težav pri prenosu lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)