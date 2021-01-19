---
title: Dodeljevanje dovoljenj
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901616"
---
# <a name="grant-permissions"></a><span data-ttu-id="84471-102">Dodeljevanje dovoljenj</span><span class="sxs-lookup"><span data-stu-id="84471-102">Grant permissions</span></span>

1. <span data-ttu-id="84471-103">**Dodeljevanje skrbniškega dovoljenja za celotno najemnika**: glejte [dodeljevanje skrbniškega dovoljenja za celotno uporabo v programu](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) za navodila po korakih za dodelitev skrbniškega dovoljenja za skrbnike prek portala Azure ad PowerShell ali iz samega poziva za privolitev.</span><span class="sxs-lookup"><span data-stu-id="84471-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="84471-104">**Dodelitev soglasja v imenu določenega uporabnika**: namesto odobritve dovoljenja za celotno organizacijo lahko skrbnik uporabi tudi [API za Microsoft Graph](https://docs.microsoft.com/graph/use-the-api) , da odobri dovoljenja za dodeljevanje dovoljenj v imenu posameznega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="84471-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="84471-105">Če želite več informacij, glejte [pridobi dostop v imenu uporabnika](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="84471-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>