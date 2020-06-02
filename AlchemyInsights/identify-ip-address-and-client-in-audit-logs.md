---
title: Identificirajte naslov IP in odjemalca v dnevniku revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508932"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="13e5b-102">Identificirajte naslov IP in odjemalca v dnevniku revizij</span><span class="sxs-lookup"><span data-stu-id="13e5b-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="13e5b-103">Naslov IP, ki ustreza dejavnosti uporabnika ali skrbnika Microsoft 365, je prikazan v dnevniku revizij.</span><span class="sxs-lookup"><span data-stu-id="13e5b-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="13e5b-104">Podatki o odjemalcu so tudi prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="13e5b-104">The client information is also logged.</span></span> <span data-ttu-id="13e5b-105">Tukaj so koraki za identifikacijo teh informacij</span><span class="sxs-lookup"><span data-stu-id="13e5b-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="13e5b-106">Prijavite se v [Microsoft 365 Security & center za skladnost](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="13e5b-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="13e5b-107">Pojdite na stran **Search**za  >  **iskanje dnevnika revizij** iskanja.</span><span class="sxs-lookup"><span data-stu-id="13e5b-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="13e5b-108">Če ste zainteresirani za določeno dejavnost, jo izberite s seznama **dejavnosti** .</span><span class="sxs-lookup"><span data-stu-id="13e5b-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="13e5b-109">Če ne, bodo vse dejavnosti vrnjene za izbranega uporabnika (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="13e5b-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="13e5b-110">**Opomba**: nekatere dejavnosti morda niso na voljo v meniju **dejavnosti** ; vendar pa bodo ti revizijski elementi vrnjeni, če je izbran **prikaz rezultatov za vse dejavnosti** (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="13e5b-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="13e5b-111">Določite uporabniško ime v polju **Uporabniki** , izberite ustrezno časovno območje za dejavnost in kliknite **Iskanje**.</span><span class="sxs-lookup"><span data-stu-id="13e5b-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="13e5b-112">V rezultatih lahko vidite naslov IP za to dejavnost v podoknu z rezultati.</span><span class="sxs-lookup"><span data-stu-id="13e5b-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="13e5b-113">Izberite zapis o reviziji, če si želite ogledati podrobne informacije v pojavnem meniju **podrobnosti** (na primer odjemalec, uporabnik, ki je izvedel dejanje itd.).</span><span class="sxs-lookup"><span data-stu-id="13e5b-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="13e5b-114">Če želite več informacij, glejte [Iskanje naslova IP računalnika, ki se uporablja za dostop do kompromitiranih računov](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="13e5b-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
