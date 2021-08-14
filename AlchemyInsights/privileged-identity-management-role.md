---
title: Privileged Identity Management vloga
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973245"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Dovoljenja niso dodeljena po aktiviranju vloge**

Ko aktivirate vlogo v programu Azure AD Privileged Identity Management (PIM), se aktiviranje morda ne bo takoj razširilo v vseh portalih, ki zahtevajo prednostno vlogo. Včasih lahko spletni predpomnjenje v portalu povzroči, da sprememba ne začne veljati takoj, tudi če se sprememba razširi.

Če vaša aktivacija zamuja, upoštevajte ta navodila:

1. Izpišite se iz portala Azure in se znova vpišite. Ko aktivirate vlogo imenika Azure AD ali vlogo vira Azure, boste videli stopnje aktivacije. Ko so vse stopnje dokončane, boste videli povezavo »Izpiši«. To povezavo lahko uporabite za odjavo. To bo rešilo večino primerov za zakasnitev aktiviranja.
2. Pri zaščiti pred vlogami preverite, ali ste navedeni kot član vloge.
3. Če aktivirate vlogo Exchange, se izpišite in se znova vpišite. Če težave ne morete odpraviti, odprite vstopnico za podporo in to zakasnite kot težavo. Če za dostop do središča za Exchange in skladnost s predpisi uporabljate svojo vlogo skrbnika za varnost in skladnost s predpisi, si oglejte naslednji korak.
4. Če aktivirate vlogo za dostop do središča za varnost in skladnost s predpisi ali če aktivirate vlogo skrbnika storitve SharePoint, boste v nekaj minutah do nekaj ur videli zakasnitev aktivacije. To je znana težava in aktivno sodelujemo s temi skupinami, da bi čim prej odpravili to težavo.

Če želite več informacij, si oglejte:

- [Aktiviranje vlog v storitvi Azure AD v storitvi PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktiviranje vlog vira storitve Azure v storitvi PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Ko deaktiviranje vloge ni odstranjeno, dovoljenja niso odstranjena ali pa aktiviranje vloge poteče**

Ko dezaktivite vlogo v imeniku Azure AD Privileged Identity Management ko poteče obdobje aktiviranja vloge, lahko pride do zakasnitve, do katere lahko še naprej dostopate.

Če je deaktiviranje zakasnjeno, upoštevajte ta navodila:

1. Če deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed the permissions are removeds, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.
2. Če je obdobje aktiviranja poteklo, vendar imate še vedno odprto sejo brskalnika, zaprite brskalnik. Vlogo lahko uporabljate še naprej, dokler te seje ne zaprete. To je znana težava in iščemo morebitni popravek za aktivno preklic posamezne seje po poteku aktiviranja.

Če se vaša zakasnitev razlikuje od teh dveh scenarijev, odprite vstopnico za podporo.
