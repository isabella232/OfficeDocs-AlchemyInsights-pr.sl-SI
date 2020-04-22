---
title: Prepoznavanje dejavnosti pravila» Prejeto «v dnevnikih revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716440"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="6c921-102">Prepoznavanje dejavnosti pravila» Prejeto «v dnevnikih revizij</span><span class="sxs-lookup"><span data-stu-id="6c921-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="6c921-103">Če si želite ogledati dogodke pravil nabiralnika (ustvarjanje, spreminjanje in brisanje pravil nabiralnika), lahko uporabite iskanje dnevnika revizij v središču Microsoft 365 Security & center za skladnost.</span><span class="sxs-lookup"><span data-stu-id="6c921-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="6c921-104">Prijavite se v [Microsoft 365 Security & center za skladnost](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="6c921-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="6c921-105">Pojdite na stran za**iskanje dnevnika revizij** **iskanja** > .</span><span class="sxs-lookup"><span data-stu-id="6c921-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="6c921-106">Izberite časovno območje v polji **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="6c921-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="6c921-107">V razdelku **dejavnosti Exchangeevega nabiralnika**preverite, ali je polje **dejavnosti** nastavljeno na **novo-inboxrule ustvari/spremeni/omogoči/onemogoči pravilo nabiralnika**.</span><span class="sxs-lookup"><span data-stu-id="6c921-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="6c921-108">Kliknite **Iskanje**.</span><span class="sxs-lookup"><span data-stu-id="6c921-108">Click **Search**.</span></span>

<span data-ttu-id="6c921-109">V rezultatih Izberite zapis o reviziji.</span><span class="sxs-lookup"><span data-stu-id="6c921-109">In the results, select an audit record.</span></span> <span data-ttu-id="6c921-110">V meniju podrobnosti kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="6c921-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6c921-111">Informacije o nastavitvah pravila nabiralnika so prikazane v polju **Parametri** .</span><span class="sxs-lookup"><span data-stu-id="6c921-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="6c921-112">Če želite več informacij, glejte [določanje, ali je uporabnik ustvaril pravilo» Prejeto «](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="6c921-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
