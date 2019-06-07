---
title: Prepoznavanje Prejeto pravilo dejavnost v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755053"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2247f-102">Prepoznavanje Prejeto pravilo dejavnost v dnevnikih nadzora</span><span class="sxs-lookup"><span data-stu-id="2247f-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2247f-103">Uporabite revizijo dnevnik Išči v varnostno & Center skladnosti razgledati Prejeto pravilo dogodkov (ustvarjanje, spreminjanje in brisanje pravila za prejeto pošto).</span><span class="sxs-lookup"><span data-stu-id="2247f-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2247f-104">Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2247f-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="2247f-105">Kliknite **Išči ter preiskave** in izberite **Išči dnevnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="2247f-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="2247f-106">Izberite datumski obseg v polji **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="2247f-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2247f-107">**Dejavnosti nabiralnik Exchange**, preverite polje **dejavnosti** nastavljeno na **New-InboxRule ustvari/spremeni/usposobiti/onesposobiti Prejeto pravilo**.</span><span class="sxs-lookup"><span data-stu-id="2247f-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2247f-108">Kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="2247f-108">Click **Search**.</span></span>

<span data-ttu-id="2247f-109">V rezultate, izberite revizijski zapis.</span><span class="sxs-lookup"><span data-stu-id="2247f-109">In the results, select an audit record.</span></span> <span data-ttu-id="2247f-110">V pojavni meni podrobnosti, kliknite **Več informacij**.</span><span class="sxs-lookup"><span data-stu-id="2247f-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2247f-111">V polju **parametre** so prikazane informacije o nastavitvah Prejeto pravilo.</span><span class="sxs-lookup"><span data-stu-id="2247f-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2247f-112">Če želite več informacij, glejte [določanje, če uporabnik, ki je ustvaril pravilo za prejeto pošto](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="2247f-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
