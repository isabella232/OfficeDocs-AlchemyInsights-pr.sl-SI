---
title: Brisanje ali obnovitev programov
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015018"
---
# <a name="delete-or-restore-applications"></a>Brisanje ali obnovitev programov

**Če želite izbrisati program iz svojega najemnika v storitvi AZURE ad**:

1. V **portalu AZURE ad** izberite **aplikacije za podjetja**. Nato poiščite in izberite aplikacijo, ki jo želite izbrisati.
2. V razdelku **upravljanje** v levem podoknu izberite **lastnosti**.
3. Izberite **Izbriši**, nato pa izberite **da** , če želite potrditi, da želite izbrisati program iz svojega najemnika v storitvi Azure ad.

Če želite več informacij o tem, kako izbrišete program, glejte [hitri začetek: brisanje programa iz najemnika storitve Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

V lupini PowerShell [odstranite-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) ukaz» cmdlet «odstrani konfiguracijske konfiguracije proxyja iz določenega programa v imeniku Azure Active Directory in lahko v celoti izbriše program, če je določen.

**Izbrisano aplikacijo lahko obnovite** z uporabo lupine PowerShell. Ko je program, ki ga želite obnoviti, identificiran, ga lahko obnovite s funkcijo» [Obnovi AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)«.
