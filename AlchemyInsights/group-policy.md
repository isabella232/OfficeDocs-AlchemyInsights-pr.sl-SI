---
title: Pravilnik skupine
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
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256906"
---
# <a name="group-policy"></a><span data-ttu-id="b5c73-102">Pravilnik skupine</span><span class="sxs-lookup"><span data-stu-id="b5c73-102">Group policy</span></span>

<span data-ttu-id="b5c73-103">Nastavitve za predmete uporabnika in računalnike v domenskih storitvah Azure Active Directory (Azure AD DS) pogosto upravljajo s predmeti pravilnika skupine (GPO-ji).</span><span class="sxs-lookup"><span data-stu-id="b5c73-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="b5c73-104">Azure AD DS vključuje vgrajene GPO-je za uporabnike AADDC in AADDC računalnike.</span><span class="sxs-lookup"><span data-stu-id="b5c73-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="b5c73-105">Te vgrajene GPO-je lahko prilagodite tako, da konfigurirate pravilnik skupine, kot je potrebno za vaše okolje.</span><span class="sxs-lookup"><span data-stu-id="b5c73-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="b5c73-106">Člani skupine» Skrbniki v storitvi Azure AD DC «imajo skrbniške pravice pravilnika skupine v domeni Azure AD DS, lahko pa tudi ustvarijo GPO in organizacijske enote po meri (organizacijske).</span><span class="sxs-lookup"><span data-stu-id="b5c73-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="b5c73-107">Če želite več informacij o tem, kaj je pravilnik skupine in kako deluje, glejte [pregled pravilnika skupine](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="b5c73-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="b5c73-108">V hibridnem okolju se pravilniki skupine, konfigurirani v okolju na mestu uporabe AD DS, ne sinhronizirajo s storitvijo Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="b5c73-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="b5c73-109">Če želite določiti nastavitve konfiguracije za uporabnike ali računalnike v storitvi Azure AD DS, uredite enega od privzetih GPO-jev ali ustvarite GPO po meri.</span><span class="sxs-lookup"><span data-stu-id="b5c73-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="b5c73-110">V tem članku je [upravljanje pravilnika skupine](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) prikazano, kako namestite orodja za upravljanje pravilnika skupine, kako lahko tone uredite vgrajene GPO-je in kako ustvarite GPO-je po meri.</span><span class="sxs-lookup"><span data-stu-id="b5c73-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



