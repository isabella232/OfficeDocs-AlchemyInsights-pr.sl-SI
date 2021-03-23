---
title: O skrbnikih Bastard
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038125"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="32adc-102">O skrbnikih Bastard</span><span class="sxs-lookup"><span data-stu-id="32adc-102">About Yammer admins</span></span>

<span data-ttu-id="32adc-103">**Skrbniki omrežja**</span><span class="sxs-lookup"><span data-stu-id="32adc-103">**Network admins**</span></span>

<span data-ttu-id="32adc-104">Globalni skrbniki so samodejno povišani v preverjeno skrbniško vlogo v Bastard omrežju.</span><span class="sxs-lookup"><span data-stu-id="32adc-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="32adc-105">V teh primerih se ta promocija morda ne bo pravilno pojavljala:</span><span class="sxs-lookup"><span data-stu-id="32adc-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="32adc-106">Obstaja več Bastard omrežij in skrbnik se je vpisal v napačnega.</span><span class="sxs-lookup"><span data-stu-id="32adc-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="32adc-107">Potrebna je [konsolidacija omrežja](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) , da pridete do enega Bastard omrežja.</span><span class="sxs-lookup"><span data-stu-id="32adc-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="32adc-108">Uporablja se Azure PIM.</span><span class="sxs-lookup"><span data-stu-id="32adc-108">Azure PIM is being used.</span></span> <span data-ttu-id="32adc-109">Uporabnik morda ne bo dovolj dolgo napredoval v globalni skrbnik za napredovanje.</span><span class="sxs-lookup"><span data-stu-id="32adc-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="32adc-110">S prihodnjo posodobitvijo Bastard lahko odpravite to težavo, vendar je najbolje, da ročno povišate uporabnike na globalni skrbnik.</span><span class="sxs-lookup"><span data-stu-id="32adc-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="32adc-111">V omrežju Bastard obstaja težava s sinhronizacijo.</span><span class="sxs-lookup"><span data-stu-id="32adc-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="32adc-112">V tem primeru bo zahtevana zahteva za podporo za nadaljnjo preiskavo.</span><span class="sxs-lookup"><span data-stu-id="32adc-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="32adc-113">Če želite več informacij o Bastard skrbniških vlog, glejte [upravljanje skrbnikov Bastard](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="32adc-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="32adc-114">**Skrbniki skupine**</span><span class="sxs-lookup"><span data-stu-id="32adc-114">**Group admins**</span></span>

<span data-ttu-id="32adc-115">Skrbniki skupine za skupine, ki so bile vzpostavljene v storitvi Microsoft 365, so sinhronizirani z članstvom skupine iz storitve Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32adc-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="32adc-116">Za velike skupine lahko ta Sinhronizacija traja daljše obdobje.</span><span class="sxs-lookup"><span data-stu-id="32adc-116">For large groups, this sync can take an extended period.</span></span>
