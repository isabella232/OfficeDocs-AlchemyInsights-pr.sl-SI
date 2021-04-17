---
title: Ustvarjanje skupine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816388"
---
# <a name="create-a-group"></a><span data-ttu-id="7d89f-102">Ustvarjanje skupine</span><span class="sxs-lookup"><span data-stu-id="7d89f-102">Create a group</span></span>

<span data-ttu-id="7d89f-103">V tej temi je opisano ustvarjanje skupin.</span><span class="sxs-lookup"><span data-stu-id="7d89f-103">This topic describes group creation.</span></span>

<span data-ttu-id="7d89f-104">**Dovoljenje za ustvarjanje skupine**</span><span class="sxs-lookup"><span data-stu-id="7d89f-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="7d89f-105">Prepričajte se, da imate dovoljenje za ustvarjanje nove skupine.</span><span class="sxs-lookup"><span data-stu-id="7d89f-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="7d89f-106">Globalni skrbniki lahko onemogočijo ustvarjanje skupin na portalu Azure ali v podoknu za dostop.</span><span class="sxs-lookup"><span data-stu-id="7d89f-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="7d89f-107">Morda boste potrebovali skrbnika, ki bo ustvaril novo skupino za vas ali vam dal ustrezna dovoljenja.</span><span class="sxs-lookup"><span data-stu-id="7d89f-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="7d89f-108">**Upravljanje dovoljenj za ustvarjanje skupine**</span><span class="sxs-lookup"><span data-stu-id="7d89f-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="7d89f-109">Globalni skrbniki lahko upravljajo dovoljenja za ustvarjanje skupin (iz varnostnih razlogov) ali skupine v storitvi Office 365, ki so ustvarjene na portalu Azure ali v podoknu za dostop tako, da izberejo »Uporabniki lahko ustvarijo varnostne skupine v portalih Azure« ali »Uporabniki lahko ustvarijo skupine v storitvi Office 365 na portalih Azure« v razdelku Vse skupine Splošno  >  **(Nastavitve)**.</span><span class="sxs-lookup"><span data-stu-id="7d89f-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="7d89f-110">Prav tako lahko omejite ustvarjanje skupin, da izberete skupino uporabnikov, če imate licenco za Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="7d89f-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="7d89f-111">**Onemogočanje pozdravnega obvestila za nove člane skupine v storitvi Office 365**</span><span class="sxs-lookup"><span data-stu-id="7d89f-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="7d89f-112">Pozdravno obvestilo, poslano uporabnikom, ki so bili dodani v skupine v storitvi Office 365, lahko onemogočite tako, da v ogrodju Powershell **UnifiedGroupWelcomeMessageEnabled** nastavite »False«.</span><span class="sxs-lookup"><span data-stu-id="7d89f-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="7d89f-113">Več o tej nastavitvi [izveste tukaj.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="7d89f-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

