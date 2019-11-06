---
title: Poročila o klasičnem SharePointovem dnevniku revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992634"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="33257-102">Dnevniki revizij v SharePointu in storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="33257-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="33257-103">Dnevniki klasičnih revizij v SharePointu</span><span class="sxs-lookup"><span data-stu-id="33257-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="33257-104">Revizija SPO je bila preseljena v dnevnik poenotenega nadzora (UAL).</span><span class="sxs-lookup"><span data-stu-id="33257-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="33257-105">Vsa podedovana revizijska poročila SPO se bodo zdaj napajala prek UAL, podedovani revizijski signali pa so bili preseljeni v UAL.</span><span class="sxs-lookup"><span data-stu-id="33257-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="33257-106">Ključne spremembe:</span><span class="sxs-lookup"><span data-stu-id="33257-106">Key changes:</span></span>

* <span data-ttu-id="33257-107">Obrezovanje ni na voljo kot zmožnost.</span><span class="sxs-lookup"><span data-stu-id="33257-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="33257-108">Izbiranje specifičnih dogodkov za revizijo ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="33257-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="33257-109">Za celoten seznam revidiranih dogodkov, ki so privzeto na voljo, glejte [ta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="33257-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="33257-110">Možnost **lokacija** pod **prilagojena poročila** ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="33257-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="33257-111">Možnosti **odpiranja ali prenosa dokumentov** ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="33257-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="33257-112">Konfiguracija nastavitev revizij za zbirko mest</span><span class="sxs-lookup"><span data-stu-id="33257-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="33257-113">Iz skladnosti se dnevniki programa SharePoint in OneDrive Modern Unified Audit</span><span class="sxs-lookup"><span data-stu-id="33257-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="33257-114">Vklop/izklop pisanja dnevnika poenotenega nadzora</span><span class="sxs-lookup"><span data-stu-id="33257-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="33257-115">V SharePointu ali storitvi OneDrive ni potrebna nobena dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="33257-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="33257-116">Uporaba iskanja dnevnika nadzora za preverjanje dejavnosti datotek, map, uporabnikov, dovoljenj:</span><span class="sxs-lookup"><span data-stu-id="33257-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="33257-117">Dejavnosti datotek in strani</span><span class="sxs-lookup"><span data-stu-id="33257-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="33257-118">Dejavnosti mape</span><span class="sxs-lookup"><span data-stu-id="33257-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="33257-119">Skupna raba in dostop do dejavnosti zahteve</span><span class="sxs-lookup"><span data-stu-id="33257-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="33257-120">Dejavnosti sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="33257-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="33257-121">Dejavnosti upravljanja spletnega mesta</span><span class="sxs-lookup"><span data-stu-id="33257-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="33257-122">Če želite več informacij o tem, kako pridobite te dogodke, glejte [iskanje dnevnika revizij](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="33257-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
