---
title: Nadzorovanje v storitvi Microsoft 365
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
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430063"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="708ef-102">Nadzorovanje v storitvi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="708ef-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="708ef-103">Tukaj je nekaj stvari, ki jih morate vedeti o nadzoru v programu Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="708ef-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="708ef-104">Skrbniške dejavnosti za Exchange so privzeto revidirane.</span><span class="sxs-lookup"><span data-stu-id="708ef-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="708ef-105">V postopku spreminjanja nadzora nabiralnika je privzeto za vse uporabnike.</span><span class="sxs-lookup"><span data-stu-id="708ef-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="708ef-106">Če želite več informacij o tem, kliknite [tukaj](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span><span class="sxs-lookup"><span data-stu-id="708ef-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="708ef-107">Do takrat, če želite navodila za ročno omogočanje za eno osebo ali celotno organizacijo, izberite gumb vklopi nadzor nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="708ef-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="708ef-108">Nabiralniki skupine Microsoft 365 in nabiralniki javnih map ne podpirajo dnevnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="708ef-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="708ef-109">Za SharePoint/OneDrive ni potrebna nobena dodatna konfiguracija za omogočeno nadzorovanje.</span><span class="sxs-lookup"><span data-stu-id="708ef-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="708ef-110">Če želite izvedeti, katere dejavnosti so nadzorovane, glejte:</span><span class="sxs-lookup"><span data-stu-id="708ef-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="708ef-111">Dejavnosti datoteke</span><span class="sxs-lookup"><span data-stu-id="708ef-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="708ef-112">Dejavnosti mape</span><span class="sxs-lookup"><span data-stu-id="708ef-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="708ef-113">[Skupna raba in Accessove dejavnosti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span><span class="sxs-lookup"><span data-stu-id="708ef-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="708ef-114">Seznam vseh nadzorovanih dejavnosti po storitvi najdete v članku [nadzorovane dejavnosti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="708ef-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
