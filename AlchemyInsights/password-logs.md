---
title: Dnevniki gesel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527182"
---
# <a name="password-logs"></a><span data-ttu-id="68541-102">Dnevniki gesel</span><span class="sxs-lookup"><span data-stu-id="68541-102">Password logs</span></span>

<span data-ttu-id="68541-103">**Imam težave z dostopom do dnevnikov nadzora ponastavljanja gesel**</span><span class="sxs-lookup"><span data-stu-id="68541-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="68541-104">Če želite odpraviti težave z dostopom do dnevnikov nadzora za ponastavitev gesla, izvedite ta korak:</span><span class="sxs-lookup"><span data-stu-id="68541-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="68541-105">Zagotovite, da ste pooblaščeni za ogled dnevnikov nadzora.</span><span class="sxs-lookup"><span data-stu-id="68541-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="68541-106">Dovolijo se le te vloge:</span><span class="sxs-lookup"><span data-stu-id="68541-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="68541-107">Globalni skrbnik</span><span class="sxs-lookup"><span data-stu-id="68541-107">Global administrator</span></span>
 - <span data-ttu-id="68541-108">Varnostni skrbnik</span><span class="sxs-lookup"><span data-stu-id="68541-108">Security administrator</span></span>
 - <span data-ttu-id="68541-109">Bralnik varnosti</span><span class="sxs-lookup"><span data-stu-id="68541-109">Security reader</span></span>

<span data-ttu-id="68541-110">**Vse dogodke za ponastavitev gesla želim videti od časa, ki sem ga sprva uvedli**</span><span class="sxs-lookup"><span data-stu-id="68541-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="68541-111">V poročilih zadnjih 30 dni se shranijo do 120.000 za ponastavitev/registracijo gesel.</span><span class="sxs-lookup"><span data-stu-id="68541-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="68541-112">Ta največja omejitev velja za uporabniški vmesnik pri prenosu datoteke CSV.</span><span class="sxs-lookup"><span data-stu-id="68541-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="68541-113">1.000.000 dogodki so na voljo prek lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="68541-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="68541-114">Če želite več informacij, si oglejte spodnje povezave:</span><span class="sxs-lookup"><span data-stu-id="68541-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="68541-115">Samopostrežni dogodki ponastavljanja gesel iz poročil v storitvi Azure AD in dogodki API</span><span class="sxs-lookup"><span data-stu-id="68541-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="68541-116">Kako prenesti dogodke za ponastavitev gesla za hitro delovanje z lupino PowerShell</span><span class="sxs-lookup"><span data-stu-id="68541-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="68541-117">**Želim izvedeti več o zmogljivostih poročanja za ponastavitev gesla**</span><span class="sxs-lookup"><span data-stu-id="68541-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="68541-118">Preverite, kdo se registrira ali ponastavlja gesla s dnevniškimi dnevniki storitve Azure AD za ponastavitev gesla v portalu Azure v razdelku **Uporabniki in skupine**.</span><span class="sxs-lookup"><span data-stu-id="68541-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="68541-119">Če želite več informacij, glejte te povezave:</span><span class="sxs-lookup"><span data-stu-id="68541-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="68541-120">Pregled poročil za ponastavitev gesla</span><span class="sxs-lookup"><span data-stu-id="68541-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="68541-121">Ogled poročil o ponastavitvi gesel v portalu Azure</span><span class="sxs-lookup"><span data-stu-id="68541-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="68541-122">Samopostrežni dogodki ponastavljanja gesel iz poročil v storitvi Azure AD in dogodki API</span><span class="sxs-lookup"><span data-stu-id="68541-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="68541-123">Kako prenesti dogodke za ponastavitev gesla za hitro delovanje z lupino PowerShell</span><span class="sxs-lookup"><span data-stu-id="68541-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


