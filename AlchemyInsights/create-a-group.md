---
title: Ustvarjanje skupine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089176"
---
# <a name="create-a-group"></a><span data-ttu-id="23934-102">Ustvarjanje skupine</span><span class="sxs-lookup"><span data-stu-id="23934-102">Create a group</span></span>

<span data-ttu-id="23934-103">V tej temi je opisana ustvarjanje skupine.</span><span class="sxs-lookup"><span data-stu-id="23934-103">This topic describes group creation.</span></span>

<span data-ttu-id="23934-104">**Dovoljenje za ustvarjanje skupine**</span><span class="sxs-lookup"><span data-stu-id="23934-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="23934-105">Zagotovite, da imate dovoljenje za ustvarjanje nove skupine.</span><span class="sxs-lookup"><span data-stu-id="23934-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="23934-106">Globalni skrbniki lahko onemogočijo ustvarjanje skupine v portalu Azure ali v Accessovi plošči.</span><span class="sxs-lookup"><span data-stu-id="23934-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="23934-107">Morda boste potrebovali skrbnika, če želite ustvariti novo skupino za vas ali pa vam dati ustrezna dovoljenja.</span><span class="sxs-lookup"><span data-stu-id="23934-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="23934-108">**Upravljanje dovoljenj za ustvarjanje skupin**</span><span class="sxs-lookup"><span data-stu-id="23934-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="23934-109">Globalni skrbniki lahko upravljajo dovoljenja za ustvarjanje skupin (zaradi varnostnih razlogov) ali skupin Office 365, ki so bile ustvarjene v portalu Azure ali Accessovi plošči, tako da izberete» uporabniki lahko ustvarijo varnostne skupine v storitvi Azure portali «ali» uporabniki lahko ustvarijo Office 365 skupine v storitvi Azure Portals «v razdelku» **vse skupine**«  >  **(nastavitve)**.</span><span class="sxs-lookup"><span data-stu-id="23934-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="23934-110">Lahko tudi omejite ustvarjanje skupine, če želite izbrati skupino uporabnikov, če imate licenco Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="23934-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="23934-111">**Onemogočanje pozdravne priglasitve za nove člane skupine v sistemu Office 365**</span><span class="sxs-lookup"><span data-stu-id="23934-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="23934-112">Pozdravno obvestilo, poslano uporabnikom, ki so dodani v skupine sistema Office 365, lahko onemogočite tako, da nastavite **UnifiedGroupWelcomeMessageEnabled** na False v lupini PowerShell.</span><span class="sxs-lookup"><span data-stu-id="23934-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="23934-113">Preberite več o tej nastavitvi [tukaj](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="23934-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

