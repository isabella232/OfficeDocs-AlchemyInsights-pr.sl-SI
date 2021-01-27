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
# <a name="delete-or-restore-applications"></a><span data-ttu-id="1f8b1-102">Brisanje ali obnovitev programov</span><span class="sxs-lookup"><span data-stu-id="1f8b1-102">Delete or restore applications</span></span>

<span data-ttu-id="1f8b1-103">**Če želite izbrisati program iz svojega najemnika v storitvi AZURE ad**:</span><span class="sxs-lookup"><span data-stu-id="1f8b1-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="1f8b1-104">V **portalu AZURE ad** izberite **aplikacije za podjetja**.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="1f8b1-105">Nato poiščite in izberite aplikacijo, ki jo želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="1f8b1-106">V razdelku **upravljanje** v levem podoknu izberite **lastnosti**.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="1f8b1-107">Izberite **Izbriši**, nato pa izberite **da** , če želite potrditi, da želite izbrisati program iz svojega najemnika v storitvi Azure ad.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="1f8b1-108">Če želite več informacij o tem, kako izbrišete program, glejte [hitri začetek: brisanje programa iz najemnika storitve Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="1f8b1-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="1f8b1-109">V lupini PowerShell [odstranite-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) ukaz» cmdlet «odstrani konfiguracijske konfiguracije proxyja iz določenega programa v imeniku Azure Active Directory in lahko v celoti izbriše program, če je določen.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="1f8b1-110">**Izbrisano aplikacijo lahko obnovite** z uporabo lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="1f8b1-111">Ko je program, ki ga želite obnoviti, identificiran, ga lahko obnovite s funkcijo» [Obnovi AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)«.</span><span class="sxs-lookup"><span data-stu-id="1f8b1-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
