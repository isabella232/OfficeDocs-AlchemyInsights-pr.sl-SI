---
title: Podprte vrste naročnin
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
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820698"
---
# <a name="supported-subscription-types"></a>Podprte vrste naročnin

Če želite nadaljevati, preglejte podprte vrste naročnin.

[Podprte vrste naročnin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prenos lastništva za obračunavanje**

Azure portal kot [Skrbnik računa](https://ms.portal.azure.com/) za obračunavanje z naročnino, ki jo želite prenesti

- Poiščete **Upravljanje stroškov in obračunavanje**. Izberite **Naročnine** v levem podoknu. Glede na dostop boste morda morali izbrati obseg obračunavanja in nato **Naročnine** ali **Naročnine Azure**.
- Za naročnino, ki jo želite prenesti, izberite Prenesi lastništvo za obračunavanje.
- Vnesite e-poštni naslov uporabnika, ki je skrbnik za obračunavanje računa, ki bo nov lastnik naročnine, nato pa izberite **pošljite zahtevo za prenos**.
- Uporabnik prejme e-poštno sporočilo z navodili za pregled vaše zahteve za prenos. Če želite odobriti zahtevo za prenos, uporabnik izbere povezavo v e-poštnem sporočilu in sledi navodilom.

Opomba: Če prenesete lastništvo računov za naročnino na uporabniški račun v drugem najemniku Azure AD, bodo vse [dodelitve nadzora dostopa (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje virov v naročnini trajno odstranjene. Za upravljanje virov v naročnini bo imel dostop le nov lastnik. Če želite več informacij o tem, glejte [Prenašanje naročnine na uporabnika v drugem najemniku storitve Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenos lastništva naročnine**

Prenos lastništva naročnine na podlagi vlog (RBAC) za upravljanje virov v naročnini izgubi dostop. Če želite več informacij o dodajanju obstoječe naročnine najemniku, glejte [Pridružitev ali dodajanje naročnine Azure v Azure Active Directory. ](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenos naročnine z obstoječim neplačanim zneskom iz trenutnega obračunskega cikla ne bo prenesen na nov plačilni instrument v novem računu. Edine informacije, ki so na voljo uporabnikom v novem računu, so stroški vaše naročnine v zadnjem mesecu. Preostala zgodovina uporabe in obračunavanja se ne prenese z naročnino.
- Prenos lastništva računov za naročnine na Enterprise Agreement (EA) je trenutno podprt samo na portalu Enterprise Agreement
- Če želite prenesti kreditno naravnano naročnino, kot so Visual Studio, BizSpark, mrežo Microsoftovih partnerjev na novega uporabnika, mora imeti licenco Visual Studio/licenco mreže Microsoftovih partnerjev za sprejem zahteve za prenos
- Vsi viri, kot so navidezni računalniki, diski in spletna mesta, se uspešno prenesejo na nov račun. Pri prenosu naročnine med najemniki bi lahko vplivali na naslednje vire:

**Domenske storitve Azure AD Domain Services**

Azure Key Vaults

- To bi lahko vplivalo [na uporabnike in zbirke podatkov, povezane s SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), še posebej, če stranka uporablja preverjanje pristnosti, povezano z Azure Active Directory
- To lahko vpliva na **storitve aplikacij**, konfigurirane z overjanjem Azure Active Directory
- Računi Storitev **Visual Studio Team**, povezani z naročninami na Azure, lahko začasno izgubijo dostop, ko prekinete povezano naročnino na Azure

**Priporočeni dokumenti**

Koraki po sprejemu lastništva računov:

- Če želite obdržati lastništvo računov, vendar spremeniti vrsto naročnine, glejte: [Preklop naročnine na Azure na drugo ponudbo](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos Visual Studio, Microsoft partner Network (MPN) in Pay as you go dev/preskusne naročnine](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos lastništva za obračunavanje naročnin za Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Pogosta vprašanja o prenosu lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Odpravljanje težav s prenosom lastništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)