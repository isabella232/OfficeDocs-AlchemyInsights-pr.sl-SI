---
title: Lokacija podatkov
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627862"
---
# <a name="data-location"></a><span data-ttu-id="311f5-102">Lokacija podatkov</span><span class="sxs-lookup"><span data-stu-id="311f5-102">Data location</span></span>

<span data-ttu-id="311f5-103">Lokacijo vašega najemnika Office 365 si lahko ogledate v skrbniškem središču ali pa s povezavo na Exchange Online prek lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="311f5-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="311f5-104">**Skrbniško središče:**</span><span class="sxs-lookup"><span data-stu-id="311f5-104">**Admin center:**</span></span>
1. <span data-ttu-id="311f5-105">Prijavite se v [skrbniško središče](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="311f5-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="311f5-106">Izberite **Nastavitve** > **organizacije profil**.</span><span class="sxs-lookup"><span data-stu-id="311f5-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="311f5-107">Pod **lokacijo podatkov**izberite **Ogled podrobnosti**.</span><span class="sxs-lookup"><span data-stu-id="311f5-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="311f5-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="311f5-108">**PowerShell:**</span></span>
1. <span data-ttu-id="311f5-109">Z lupino Windows PowerShell vzpostavite povezavo s storitvijo Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="311f5-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="311f5-110">Izvršiti [zaslužiti-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet razpoložiti a zapisati v seznam od vaš najemnik ' premožen.</span><span class="sxs-lookup"><span data-stu-id="311f5-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="311f5-111">Poglejte lastnost OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="311f5-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="311f5-112">Ko imate podatkovno lokacijo za EXO in SPO, lahko določite lokacijo podatkov za druge storitve, ki jih lahko uporabljate od koder se [nahajajo vaši podatki](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="311f5-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>