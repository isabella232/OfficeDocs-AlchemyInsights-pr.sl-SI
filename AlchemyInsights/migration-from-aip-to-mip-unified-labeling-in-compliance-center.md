---
title: Selitev iz AIP v MIP/enotno označevanje v središču za skladnost
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674342"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Selitev iz AIP v MIP/enotno označevanje v središču za skladnost

Če želite preseliti iz oznak AIP na enotno označevanje v središču za varnost in skladnost s predpisi, naredite to:

**Aktiviranje zaščite v portalu Azure**

1. Če tega še niste storili, odprite novo okno brskalnika in se [vpišite v portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Pomaknite se do rezila za **zaščito informacij Azure** . V meniju zvezdišče na primer kliknite **vse storitve** in začnite vnašati **podatke** v polje filter. Izberite **zaščita za Azure Information**. Če še niste dostopali do rezila za zaščito informacij Azure, si oglejte enkratne [dodatne korake](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) za dodajanje tega rezila v portal. Če želite odpreti rezilo za zaščito informacij Azure, morate imeti [paket Premium za zaščito](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) informacij ali paket Office 365, ki vključuje upravljanje pravic. Če imate eno od teh naročnin, vendar se prikaže sporočilo, da ni mogoče najti veljavne naročnine, se [obrnite na Microsoftovo podporo](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ali uporabite standardne kanale za podporo.

2. Poiščite možnosti za **upravljanje** menija in izberite **aktivacija zaščite**. Kliknite **Aktiviraj**in potrdite dejanje. Ko je aktiviranje dokončano, vrstica z informacijami prikaže **uspešno dokončano aktiviranje**.

**Selitev oznak za zaščito informacij Azure v Office 365 Security Center za skladnost s predpisi &**

1. Prepričajte se, da ste prijavljeni kot uporabnik z dovoljenjem globalnega skrbnika.

2. Pomaknite se do rezila za **zaščito informacij Azure** .

3. V možnosti» **Upravljaj** meni «izberite **poenoteno označevanje**.

4. Na rezilu z **oznako Azure Information-enotno označevanje** kliknite **Aktiviraj** in sledite spletnim navodilom.

**Opomba**: Preverite, ali imate ustrezna dovoljenja, preden aktivirate selitveni center za skladnost varnostnega &. Če želite več informacij, si oglejte te članke:

1. [Ali morate biti globalni skrbnik, če želite konfigurirati zaščito informacij Azure ali lahko prenesem na druge skrbnike?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Pomembne informacije o skrbniških vlogah po selitvi v središče za skladnost s predpisi o varnosti &.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Če želite več informacij o AIP za poenoteno označevanje selitve v središče za varnost in skladnost s predpisi, glejte [selitev nalepk](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
