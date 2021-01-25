---
title: Preslikava atributov uporabnika za omogočanje uporabe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949896"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="5adff-102">Preslikava atributov uporabnika za omogočanje uporabe</span><span class="sxs-lookup"><span data-stu-id="5adff-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="5adff-103">Za odpravljanje težav z znanimi težavami pri preslikavi atributov glejte [preslikave atributov](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="5adff-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="5adff-104">Microsoft Azure Active Directory (AD) zagotavlja podporo za omogočanje uporabe uporabnika za aplikacije SaaS, kot je platforme Salesforce, G Suite in drugi.</span><span class="sxs-lookup"><span data-stu-id="5adff-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="5adff-105">Če omogočite omogočanje uporabe uporabnika za uporabo storitve SaaS, portal Azure nadzoruje svoje vrednosti atributov prek preslikav atributov.</span><span class="sxs-lookup"><span data-stu-id="5adff-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="5adff-106">Če želite izvedeti, kako prilagodite privzete preslikave atributov, si oglejte [prilagajanje atributov za omogočanje uporabe uporabnikov v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="5adff-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="5adff-107">Če želite izvedeti več o omogočanju uporabe uporabnikov aplikacije SaaS, glejte [Kaj je avtomatizirano omogočanje uporabe uporabnikov v storitvi AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="5adff-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="5adff-108">Ko prilagodite preslikave atributov za omogočanje uporabe uporabnika, boste morda ugotovili, da atribut, ki ga želite preslikati, ni prikazan na seznamu izvorni atribut.</span><span class="sxs-lookup"><span data-stu-id="5adff-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="5adff-109">[Sinhronizacija atributa iz imenika Active Directory v storitvi AZURE ad za omogočanje uporabe v članku aplikacije](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) vam pokaže, kako dodati manjkajoči atribut tako, da ga sinhronizirate z oglasa na mestu uporabe v storitvi Azure ad.</span><span class="sxs-lookup"><span data-stu-id="5adff-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
