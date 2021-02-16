---
title: Sinhronizacija skupine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256917"
---
# <a name="group-sync"></a><span data-ttu-id="3277a-102">Sinhronizacija skupine</span><span class="sxs-lookup"><span data-stu-id="3277a-102">Group sync</span></span>

<span data-ttu-id="3277a-103">V tem članku so navodila za sinhronizacijo skupine.</span><span class="sxs-lookup"><span data-stu-id="3277a-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="3277a-104">Če globalni skrbnik ali lastnik skupine ne more spremeniti lastnosti skupine ali dodati članov ali dodeliti lastnikov v portalu Azure, zagotovite, da je vir avtoritete za skupino v storitvi Azure Active Directory (Azure AD) za globalni skrbnik ali lastnik skupine, če želite spremeniti skupino.</span><span class="sxs-lookup"><span data-stu-id="3277a-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="3277a-105">Preden poskusite izbrisati sinhronizirano skupino v storitvi Azure AD, poskrbite, da boste [izbrisali vse dodeljene licence](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) , da se izognete napakam.</span><span class="sxs-lookup"><span data-stu-id="3277a-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="3277a-106">Če želite razumeti, kako sinhronizirati uporabnike, skupine in stike, si oglejte [sinhronizacija storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)in sledite [sinhronizaciji skupine na](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) mestu uporabe v storitvi Azure ad Connect s povezavo s sinhronizacijo v skupinah s funkcijo ad Connect.</span><span class="sxs-lookup"><span data-stu-id="3277a-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="3277a-107">S tem vodnikom lahko odpravite [napake pri sinhronizaciji](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) , če želite odpraviti pogoste napake med sinhronizacijo.</span><span class="sxs-lookup"><span data-stu-id="3277a-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

