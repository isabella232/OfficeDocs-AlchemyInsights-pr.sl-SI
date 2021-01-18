---
title: Sinhronizacija storitve Domain
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885563"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="18c3e-102">Sinhronizacija storitve Domain</span><span class="sxs-lookup"><span data-stu-id="18c3e-102">Domain service synchronization</span></span>

<span data-ttu-id="18c3e-103">Predmeti in poverilnice v domenskih storitvah storitve Azure Active Directory (Azure AD DS) lahko ustvarite lokalno v domeni ali pa se sinhronizirajo iz najemnika Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="18c3e-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="18c3e-104">Ko prvič uvedete Azure AD DS, je Samodejna enosmerna sinhronizacija konfigurirana in zagnana, da replicira predmete iz storitve Azure AD.</span><span class="sxs-lookup"><span data-stu-id="18c3e-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="18c3e-105">Ta enosmerna sinhronizacija se še naprej izvaja v ozadju, če želite ohraniti domeno Azure AD DS, ki je upravljana z vsemi spremembami iz storitve Azure AD.</span><span class="sxs-lookup"><span data-stu-id="18c3e-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="18c3e-106">Do sinhronizacije v storitvi Azure AD DS se ne prikaže nobena sinhronizacija.</span><span class="sxs-lookup"><span data-stu-id="18c3e-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="18c3e-107">Če želite več podrobnosti o sinhronizaciji domenske storitve Azure Active Directory, glejte [sinhronizacija storitve Domain](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="18c3e-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
