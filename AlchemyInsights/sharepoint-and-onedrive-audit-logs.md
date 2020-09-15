---
title: Poročila iz klasičnega SharePointovega dnevnika nadzora
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662224"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="d84bd-102">SharePoint in OneDrive dnevniki nadzora</span><span class="sxs-lookup"><span data-stu-id="d84bd-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="d84bd-103">SharePoint Classic Audit dnevniki</span><span class="sxs-lookup"><span data-stu-id="d84bd-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="d84bd-104">SPO Legacy Audit je bil preseljen v poenoteni dnevnik nadzora (UAL).</span><span class="sxs-lookup"><span data-stu-id="d84bd-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="d84bd-105">Vsa SPO podedovana poročila o nadzoru bodo zdaj napajana prek UAL, območni revizijski signali pa so preseljeni v UAL.</span><span class="sxs-lookup"><span data-stu-id="d84bd-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="d84bd-106">Ključne spremembe:</span><span class="sxs-lookup"><span data-stu-id="d84bd-106">Key changes:</span></span>

* <span data-ttu-id="d84bd-107">Obrezovanje ni na voljo kot zmogljivost.</span><span class="sxs-lookup"><span data-stu-id="d84bd-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="d84bd-108">Izbira določenih dogodkov za nadzor ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="d84bd-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="d84bd-109">Oglejte si [ta dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) za popoln seznam nadzorovanih dogodkov, ki so na voljo privzeto.</span><span class="sxs-lookup"><span data-stu-id="d84bd-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="d84bd-110">Možnost» **mesto** «v razdelku» **poročila po meri** «ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="d84bd-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="d84bd-111">Možnost» **odpiranje ali prenos dokumentov** «ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="d84bd-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="d84bd-112">Konfiguracija nastavitev nadzora za zbirko mest</span><span class="sxs-lookup"><span data-stu-id="d84bd-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="d84bd-113">SharePoint in OneDrive sodobni enotni dnevniki nadzora iz skladnosti</span><span class="sxs-lookup"><span data-stu-id="d84bd-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="d84bd-114">Vklop/izklop poenotenega pisanja dnevnika nadzora</span><span class="sxs-lookup"><span data-stu-id="d84bd-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="d84bd-115">V SharePointu ali OneDrive ni potrebna nobena dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="d84bd-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="d84bd-116">Če želite preveriti dejavnost datotek, map (ov), uporabnikov (ov), dovoljenj:</span><span class="sxs-lookup"><span data-stu-id="d84bd-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="d84bd-117">Dejavnosti datoteke in strani</span><span class="sxs-lookup"><span data-stu-id="d84bd-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="d84bd-118">Dejavnosti mape</span><span class="sxs-lookup"><span data-stu-id="d84bd-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="d84bd-119">Dejavnosti zahteve za skupno rabo in dostop</span><span class="sxs-lookup"><span data-stu-id="d84bd-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="d84bd-120">Dejavnosti sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="d84bd-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="d84bd-121">Dejavnosti skrbništva mesta</span><span class="sxs-lookup"><span data-stu-id="d84bd-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="d84bd-122">Če želite več informacij o tem, kako pridobite te dogodke, si oglejte [iskanje dnevnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d84bd-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
