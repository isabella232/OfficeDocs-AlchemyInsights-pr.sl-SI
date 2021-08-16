---
title: Selitev iz programa AIP v mip/poenoteno označevanje v središču za skladnost s predpisi
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
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000372"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Selitev iz programa AIP v mip/poenoteno označevanje v središču za skladnost s predpisi

Če želite oznake AIP preseliti v poenoteno označevanje v središču za varnost in skladnost s predpisi, naredite to:

**Aktiviranje zaščite s portala Azure**

1. Če tega še niste naredili, odprite novo okno brskalnika in se [vpišite v portal Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Pomaknite se do **re žetice Azure Information Protection.** V meniju zvezdišča na primer kliknite **Vse storitve** in začnite vnašati **Informacije** v polje Filter. Izberite **Azure Information Protection**. Če še niste dostopali do re naročnine na Azure Information Protection, si oglejte enkratne dodatne korake za dodajanje [tega](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) re bladea v portal. Če želite odpreti re naročnino za Azure Information Protection, morate imeti paket [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ali paket Office 365, ki vključuje storitev Rights Management. Če imate eno od teh naročnin, vendar se prikaže sporočilo, da veljavne naročnine ni mogoče [najti,](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) se obrnite na Microsoftovo podporo ali uporabite standardne kanale podpore.

2. Poiščite možnosti **menija** Upravljanje in izberite **Zaščita za aktiviranje**. Kliknite **Aktiviraj** in potrdite dejanje. Po dokončanem aktiviranju je v vrstici z informacijami **prikazano, da je aktiviranje uspešno dokončano.**

**Selitev oznak Azure Information Protection v središče Office 365 za & s predpisi**

1. Prepričajte se, da ste prijavljeni kot uporabnik z dovoljenjem globalnega skrbnika.

2. Pomaknite se do **re žetice Azure Information Protection.**

3. V **meniju** Upravljaj izberite **Poenoteno označevanje**.

4. V re **bladeu Azure Information Protection – poenoteno označevanje** kliknite **Aktiviraj** in upoštevajte spletna navodila.

**Opomba:** Preverite, ali imate ustrezna dovoljenja, preden aktivirate selitev središča za & s predpisi. Več informacij najdete v teh člankih:

1. [Ali morate biti globalni skrbnik, če želite konfigurirati Azure Information Protection, ali sem lahko pooblaščen drugim skrbnikom?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Pomembne informacije o skrbniških vlogah po selitvi v središče za & s predpisi.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Če želite več informacij o selitvi AIP v poenoteno označevanje v središče za varnost in skladnost s predpisi, glejte [Selitev oznak.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
