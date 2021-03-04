---
title: Iskanje naslova IP v dnevniku nadzora
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429791"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="c92de-102">Iskanje naslova IP v dnevniku nadzora</span><span class="sxs-lookup"><span data-stu-id="c92de-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="c92de-103">Naslov IP, ki ustreza dejavnosti, ki jo izvaja uporabnik ali skrbnik, je prikazan v dnevnikih nadzora.</span><span class="sxs-lookup"><span data-stu-id="c92de-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="c92de-104">Podatki odjemalca so tudi prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="c92de-104">The client information is also logged.</span></span> <span data-ttu-id="c92de-105">Tukaj je, kako prepoznate naslov IP:</span><span class="sxs-lookup"><span data-stu-id="c92de-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="c92de-106">Obiščite središče za [skladnost z varnostnim &om sistema Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="c92de-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="c92de-107">Izberite   >  **[iskanje dnevnika nadzora](https://go.microsoft.com/fwlink/?linkid=2103759)** iskanja.</span><span class="sxs-lookup"><span data-stu-id="c92de-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="c92de-108">Če opazite obvestilo, ki ga morate vklopiti, ga vklopite zdaj.</span><span class="sxs-lookup"><span data-stu-id="c92de-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="c92de-109">Če ta funkcija ni omogočena, rezultati iskanja ne bodo mogli povleči podatkov iz prejšnjih datumov.</span><span class="sxs-lookup"><span data-stu-id="c92de-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="c92de-110">Če vas zanima določena dejavnost, jo izberite na seznamu **dejavnosti** ; v nasprotnem primeru bodo privzeto vse dejavnosti vrnjene za izbranega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="c92de-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="c92de-111">Upoštevajte, da nekatere dejavnosti morda ne bodo na voljo za izbor v meniju **dejavnosti** ; vendar pa bodo ti revizijski elementi vrnjeni, če je izbrana možnost **Pokaži rezultate za vse dejavnosti** (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="c92de-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="c92de-112">Določite datumski obseg in v polju **Uporabniki** izberite uporabniško ime za uporabnika, ki ga želite raziskati.</span><span class="sxs-lookup"><span data-stu-id="c92de-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="c92de-113">Izberite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="c92de-113">Select **Search**.</span></span> <span data-ttu-id="c92de-114">Dejavnosti so prikazane v razdelku **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="c92de-114">The activities appear under **Results**.</span></span> <span data-ttu-id="c92de-115">Naslov IP za vsako dejavnost si lahko ogledate.</span><span class="sxs-lookup"><span data-stu-id="c92de-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="c92de-116">Če si želite ogledati podrobnosti, izberite dejavnost in nato izberite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="c92de-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="c92de-117">Če želite izvedeti več, glejte Iskanje v [dnevniku nadzora sistema Office 365 za odpravljanje pogostih scenarijev](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="c92de-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>