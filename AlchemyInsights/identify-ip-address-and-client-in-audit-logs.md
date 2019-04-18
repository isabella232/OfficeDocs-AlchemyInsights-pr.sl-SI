---
title: Prepoznati IP naslov odjemalca v dnevnikih nadzora in
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909563"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="af4fb-102">Prepoznati IP naslov odjemalca v dnevnikih nadzora in</span><span class="sxs-lookup"><span data-stu-id="af4fb-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="af4fb-103">IP naslov, ki ustreza dejavnost uporabnika ali skrbnik je prikazan v dnevnikov.</span><span class="sxs-lookup"><span data-stu-id="af4fb-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="af4fb-104">Zabeleženo je tudi odjemalec informacije.</span><span class="sxs-lookup"><span data-stu-id="af4fb-104">The client information is also logged.</span></span> <span data-ttu-id="af4fb-105">Tu so koraki za prepoznavanje teh informacij</span><span class="sxs-lookup"><span data-stu-id="af4fb-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="af4fb-106">Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="af4fb-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="af4fb-107">Kliknite **Išči ter preiskave** in izberite **Išči dnevnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="af4fb-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="af4fb-108">Če ste zainteresirani za posebne dejavnosti, ga izberite iz seznama **dejavnosti** .</span><span class="sxs-lookup"><span data-stu-id="af4fb-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="af4fb-109">Če ne, se izpišejo vse dejavnosti za izbranega uporabnika (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="af4fb-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="af4fb-110">**Opomba**: nekatere dejavnosti ne sme biti na voljo v meniju **dejavnosti** ; vendar pa navedeni revizijski elementi izpišejo, če **Prikaži rezultate za vse dejavnosti** je izbrano (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="af4fb-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="af4fb-111">V polju **Uporabniki** določite uporabniško ime, izberite ustrezno časovno obdobje za dejavnost, in nato kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="af4fb-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="af4fb-112">V rezultatih, lahko vidite IP naslov za to dejavnost v podoknu z rezultati.</span><span class="sxs-lookup"><span data-stu-id="af4fb-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="af4fb-113">Izberite revizijski zapis podrobne informacije v **podrobnosti** flyout (primer varovanec, uporabnik, ki izvede dejanje, itd.).</span><span class="sxs-lookup"><span data-stu-id="af4fb-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="af4fb-114">Če želite več informacij, glejte [Iskanje naslova IP računalnika za dostop do ogrožena račun](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="af4fb-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
