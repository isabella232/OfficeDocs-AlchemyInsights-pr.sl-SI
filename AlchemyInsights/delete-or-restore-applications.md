---
title: Brisanje ali obnavljanje programov
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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102587"
---
# <a name="delete-or-restore-applications"></a>Brisanje ali obnavljanje programov

**Če želite izbrisati aplikacijo iz najemnika Azure AD:**

1. V **portalu za Azure AD** izberite **Aplikacije za podjetja**. Nato poiščite in izberite program, ki ga želite izbrisati.
2. V levem **podoknu** v razdelku Upravljanje izberite **Lastnosti**.
3. Izberite **Izbriši**, nato pa izberite **Da,** da potrdite brisanje aplikacije iz najemnika Imenika Azure AD.

Če želite več informacij o tem, kako izbrišete aplikacijo, glejte Hitri začetek: brisanje programa [iz najemnika Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

V storitvi PowerShell ukaz »cmdlet« [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) odstrani konfiguracije proxy aplikacije iz določene aplikacije v storitvi Azure Active Directory in lahko v celoti izbriše aplikacijo, če je določena.

Izbrisano **aplikacijo lahko obnovite z** lupino PowerShell. Ko program, ki ga želite obnoviti, identificiran, ga lahko obnovite z [ukazom Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
