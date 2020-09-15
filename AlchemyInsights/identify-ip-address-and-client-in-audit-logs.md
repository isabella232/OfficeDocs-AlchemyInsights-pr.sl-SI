---
title: Prepoznavanje naslovov IP in odjemalca v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668326"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="d9f1c-102">Prepoznavanje naslovov IP in odjemalca v dnevnikih nadzora</span><span class="sxs-lookup"><span data-stu-id="d9f1c-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="d9f1c-103">Naslov IP, ki ustreza dejavnosti, ki jo uporablja Microsoft 365 uporabnik ali skrbnik, je prikazan v dnevnikih nadzora.</span><span class="sxs-lookup"><span data-stu-id="d9f1c-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="d9f1c-104">Podatki odjemalca so tudi prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="d9f1c-104">The client information is also logged.</span></span> <span data-ttu-id="d9f1c-105">Tukaj so navodila za prepoznavanje teh informacij</span><span class="sxs-lookup"><span data-stu-id="d9f1c-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="d9f1c-106">Prijavite se v središče za preverjanje [varnosti & za skladnost s predpisi Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="d9f1c-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="d9f1c-107">Pojdite na stran **Search**  >  **iskanje dnevnika nadzora** iskanja.</span><span class="sxs-lookup"><span data-stu-id="d9f1c-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="d9f1c-108">Če vas zanima določena dejavnost, jo izberite na seznamu **dejavnosti** .</span><span class="sxs-lookup"><span data-stu-id="d9f1c-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="d9f1c-109">V nasprotnem primeru bodo vse dejavnosti vrnjene za izbranega uporabnika (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="d9f1c-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="d9f1c-110">**Opomba**: nekatere dejavnosti morda niso na voljo v meniju **dejavnosti** ; vendar pa bodo ti revizijski elementi vrnjeni, če je izbrana možnost **Pokaži rezultate za vse dejavnosti** (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="d9f1c-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="d9f1c-111">Določite uporabniško ime v polju **Uporabniki** izberite ustrezen datumski obseg za dejavnost in nato kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="d9f1c-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="d9f1c-112">V rezultatih lahko v podoknu z rezultati vidite naslov IP za to dejavnost.</span><span class="sxs-lookup"><span data-stu-id="d9f1c-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="d9f1c-113">Izberite zapis nadzora, če si želite ogledati podrobne informacije v flyout **podrobnosti** (na primer odjemalec, uporabnik, ki je opravil dejanje itd.).</span><span class="sxs-lookup"><span data-stu-id="d9f1c-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="d9f1c-114">Če želite več informacij, glejte [Iskanje naslova IP računalnika, ki se uporablja za dostop do poškodovanega računa](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="d9f1c-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
