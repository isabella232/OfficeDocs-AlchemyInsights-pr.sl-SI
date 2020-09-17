---
title: Prepoznavanje dejavnosti pravila mape» Prejeto «v dnevnikih nadzora
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779067"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="7ca92-102">Prepoznavanje dejavnosti pravila mape» Prejeto «v dnevnikih nadzora</span><span class="sxs-lookup"><span data-stu-id="7ca92-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="7ca92-103">Z iskanjem dnevnika nadzora v središču za varnost & skladnost s predpisi Microsoft 365 si lahko ogledate dogodke pravila za mapo» Prejeto «(ustvarjanje, spreminjanje in brisanje pravil za mapo» Prejeto «).</span><span class="sxs-lookup"><span data-stu-id="7ca92-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="7ca92-104">Prijavite se v središče za preverjanje [varnosti & za skladnost s predpisi Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="7ca92-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="7ca92-105">Pojdite na stran **Search**  >  **iskanje dnevnika nadzora** iskanja.</span><span class="sxs-lookup"><span data-stu-id="7ca92-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="7ca92-106">Izberite datumski obseg v poljih **Začetni datum** in **končni datum** .</span><span class="sxs-lookup"><span data-stu-id="7ca92-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="7ca92-107">V razdelku **dejavnosti nabiralnika v storitvi Exchange**preverite, ali je polje **dejavnosti** nastavljeno na **novo InboxRule ustvarjanje/spreminjanje/omogoči/onemogoči pravilo mape» Prejeto «**.</span><span class="sxs-lookup"><span data-stu-id="7ca92-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="7ca92-108">Kliknite **Išči**.</span><span class="sxs-lookup"><span data-stu-id="7ca92-108">Click **Search**.</span></span>

<span data-ttu-id="7ca92-109">V rezultatih Izberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="7ca92-109">In the results, select an audit record.</span></span> <span data-ttu-id="7ca92-110">V razdelku podrobnosti flyout kliknite **več informacij**.</span><span class="sxs-lookup"><span data-stu-id="7ca92-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="7ca92-111">Informacije o nastavitvah pravil za mapo» Prejeto «so prikazane v polju» **Parametri** «.</span><span class="sxs-lookup"><span data-stu-id="7ca92-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="7ca92-112">Če želite več informacij, glejte [določanje, ali je uporabnik ustvaril pravilo za mapo» Prejeto «](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="7ca92-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
