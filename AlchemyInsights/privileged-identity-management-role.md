---
title: Prednostna vloga za upravljanje identitete
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089151"
---
# <a name="privileged-identity-managementpim-role"></a>Vloga za upravljanje s privilegirano identiteto (PIM)

**Dovoljenja niso dodeljena po aktivaciji vloge**

Ko aktivirate vlogo v sistemu za upravljanje identitete v storitvi Azure AD (PIM), se aktiviranje morda ne bo takoj razširilo na vse portale, ki zahtevajo privilegirano vlogo. Tudi če je sprememba razširjena, lahko spletno predpomnjenje v portalu povzroči, da sprememba ne začne veljati takoj.

Če je aktivacija odložena, upoštevajte ta navodila:

1. Izpišite se iz portala Azure in se nato znova vpišite. Ko aktivirate vlogo Azure AD ali vlogo Azure Resource, boste videli faze aktiviranja. Ko so vse faze dokončane, se prikaže povezava» izpis «. To povezavo lahko uporabite, če se želite izpisati. To bo rešilo večino primerov za zakasnitev aktiviranja.
2. V storitvi PIM preverite, ali ste navedeni kot član vloge.
3. Če aktivirate vlogo skrbnika strežnika Exchange, se prepričajte, da ste se odjavili in se znova prijavili. Če težave ne morete odpraviti, odprite vstopnico za podporo in jo dvignite kot težavo. Če uporabljate svojo vlogo skrbnika Exchangea za dostop do središča za varnost in skladnost s predpisi, glejte naslednji korak.
4. Če aktivirate vlogo za dostop do središča za varnost in skladnost s predpisi ali če aktivirate vlogo skrbnika za SharePoint, boste nekaj minut odpravili z zakasnitvijo do nekaj ur. To je znana težava in aktivno sodelujemo s temi ekipami, da to težavo odpravimo čimprej.

Če želite več informacij, si oglejte:

- [Aktiviranje vlog» Azure AD «v sistemu PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivacija mojih vlog» Azure Resource «v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Dovoljenja niso odstranjena, ko deaktivirate vlogo ali pa poteče aktiviranje vloge**

Ko deaktivirate vlogo v privilegiranem upravljanju identitete v storitvi Azure AD ali ko poteče obdobje aktiviranja vloge, je morda prišlo do zakasnitve, kjer boste še naprej imeli dostop.

Če je vaša Deaktivacija odložena, upoštevajte ta navodila:

1. Če deaktivirate vlogo skrbnika strežnika Exchange ali poteče obdobje aktiviranja vloge, in opazite veliko zamudo, preden so dovoljenja odstranjena, odprite vstopnico za podporo in povejte inženirju za podporo, da vam pomaga vložiti vstopnico za ekipo za upravljanje privilegiranega dostopa (PAM) v storitvi Office o tej težavi.
2. Če je obdobje aktiviranja poteklo, vendar imate še vedno odprto sejo brskalnika, zaprite brskalnik. Vlogo lahko še naprej uporabljate, dokler ne zaprete te seje. To je znana težava, ki jo lahko odpravite tako, da aktivno ukine vsako sejo, ko je aktiviranje poteklo.

Če se zamuda razlikuje od teh dveh scenarijev, odprite vstopnico za podporo.
