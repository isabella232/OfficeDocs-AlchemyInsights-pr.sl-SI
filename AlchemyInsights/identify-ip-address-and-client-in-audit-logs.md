---
title: Prepoznati IP naslov odjemalca v dnevnikih nadzora in
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539045"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="38e23-102">Prepoznati IP naslov odjemalca v dnevnikih nadzora in</span><span class="sxs-lookup"><span data-stu-id="38e23-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="38e23-103">IP naslov, ki ustreza dejavnosti z Office 365 uporabnik ali oskrbnik je prikazan v dnevnikov.</span><span class="sxs-lookup"><span data-stu-id="38e23-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="38e23-104">Zabeleženo je tudi odjemalec informacije.</span><span class="sxs-lookup"><span data-stu-id="38e23-104">The client information is also logged.</span></span> <span data-ttu-id="38e23-105">Tu so koraki za prepoznavanje teh informacij</span><span class="sxs-lookup"><span data-stu-id="38e23-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="38e23-106">Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="38e23-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="38e23-107">Pojdi na **Iskanje** > **revizije dnevnik iskalna** stran.</span><span class="sxs-lookup"><span data-stu-id="38e23-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="38e23-108">Če ste zainteresirani za posebne dejavnosti, ga izberite iz seznama **dejavnosti** .</span><span class="sxs-lookup"><span data-stu-id="38e23-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="38e23-109">Če ne, se izpišejo vse dejavnosti za izbranega uporabnika (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="38e23-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="38e23-110">**Opomba**: nekatere dejavnosti ne sme biti na voljo v meniju **dejavnosti** ; vendar pa navedeni revizijski elementi izpišejo, če **Prikaži rezultate za vse dejavnosti** je izbrano (privzeta nastavitev).</span><span class="sxs-lookup"><span data-stu-id="38e23-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="38e23-111">V polju **Uporabniki** določite uporabniško ime, izberite ustrezno časovno obdobje za dejavnost, in nato kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="38e23-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="38e23-112">V rezultatih, lahko vidite IP naslov za to dejavnost v podoknu z rezultati.</span><span class="sxs-lookup"><span data-stu-id="38e23-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="38e23-113">Izberite revizijski zapis podrobne informacije v **podrobnosti** flyout (primer varovanec, uporabnik, ki izvede dejanje, itd.).</span><span class="sxs-lookup"><span data-stu-id="38e23-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="38e23-114">Če želite več informacij, glejte [Iskanje naslova IP računalnika za dostop do ogrožena račun](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="38e23-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
