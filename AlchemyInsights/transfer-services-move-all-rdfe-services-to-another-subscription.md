---
title: Prenos storitev – premaknite vse storitve RDFE v drugo naročnino
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692177"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Prenos storitev – premaknite vse storitve RDFE v drugo naročnino

**Premikanje virov**

Vire Azure lahko premaknete v drugo naročnino na Azure ali skupino virov pod isto naročnino z uporabo portala Azure, Azure PowerShell, Azure CLI ali ostali API za premikanje virov.

Preden lahko premikate vire, glejte:

- [Kontrolni seznam pred premikanjem virov](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Storitve, ki jih je mogoče premakniti](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preverjanje veljavnosti selitve](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Premikanje navodil za storitve](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Če želite premakniti obstoječe vire v drugo skupino virov ali naročnino, lahko uporabite:

- [Portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [PREOSTALI API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Vadnica: [premikanje virov Azure v drugo skupino virov ali naročnino](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Odpravljanje napak v programu Azure Resource Manager**

Oglejte si spodnje članke, če želite izvedeti več o nekaterih pogostih napakah uvedbe Azure in prejemati informacije, da jih razrešite. Če ne najdete kode napake pri uvedbi napake, glejte [Iskanje kode napake](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Odpravljanje napak pri uvajanju](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Odpravljanje težav s premikanjem virov Azure v novo skupino virov ali naročnino](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Če želite nadgraditi naročnino na Azure, kot je na primer preklop iz brezplačnega plačila na as-you-go, boste morali pretvoriti naročnino.

- Če želite nadgraditi brezplačno preskusno različico, si oglejte razdelek [Nadgradnja brezplačne preskusne različice ali naročnine na Microsoft Imagine Azure, da bo plačljiva](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Če želite spremeniti račun» Plačaj kot vi-go «, glejte [Spreminjanje naročnine na vašo uporabo v storitvi Azure Pay – as-you-go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Če želite dodati ali povezati naročnino na Azure za najemnika storitve Azure Active Directory:**

1. Vpišite se in izberite naročnino, ki jo želite uporabiti, na strani» naročnine « [v portalu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Izberite **Spremeni imenik**.
3. Preglejte vsa opozorila, ki se prikažejo, nato pa izberite **Spremeni**.
4. Imenik je spremenjen za naročnino in prejeli boste sporočilo o uspehu.
5. Če se želite premakniti v nov imenik, uporabite preklopnik *imenika* . Lahko traja do 10 minut, če želite, da se vse prikaže pravilno.

**Priporočeni dokumenti**

- [Prenos lastništva naročnine na Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Premikanje virov v novo skupino virov ali naročnino](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Upravljanje virov z uporabo portala Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
