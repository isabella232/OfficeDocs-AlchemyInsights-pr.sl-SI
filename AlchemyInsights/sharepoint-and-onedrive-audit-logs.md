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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068039"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="51091-102">Dnevniki revizij v SharePointu in storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="51091-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="51091-103">**Iz skladnosti se dnevniki programa SharePoint in OneDrive Modern Unified Audit**</span><span class="sxs-lookup"><span data-stu-id="51091-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="51091-104">Vklop/izklop pisanja dnevnika poenotenega nadzora</span><span class="sxs-lookup"><span data-stu-id="51091-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="51091-105">V SharePointu ali storitvi OneDrive ni potrebna nobena dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="51091-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="51091-106">Uporaba iskanja dnevnika nadzora za preverjanje dejavnosti datotek, map, uporabnikov, dovoljenj:</span><span class="sxs-lookup"><span data-stu-id="51091-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="51091-107">Dejavnosti datotek in strani</span><span class="sxs-lookup"><span data-stu-id="51091-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="51091-108">Dejavnosti mape</span><span class="sxs-lookup"><span data-stu-id="51091-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="51091-109">Skupna raba in dostop do dejavnosti zahteve</span><span class="sxs-lookup"><span data-stu-id="51091-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="51091-110">Dejavnosti sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="51091-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="51091-111">Dejavnosti upravljanja spletnega mesta</span><span class="sxs-lookup"><span data-stu-id="51091-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="51091-112">Če želite več informacij o tem, kako pridobite te dogodke, glejte [iskanje dnevnika revizij](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="51091-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="51091-113">**Dnevniki klasičnih revizij v SharePointu**</span><span class="sxs-lookup"><span data-stu-id="51091-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="51091-114">V dnevnik poenotenih revizij (UAL) smo preselili starejšo revizijo SPO.</span><span class="sxs-lookup"><span data-stu-id="51091-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="51091-115">To v bistvu pomeni, da se bodo vsa zapuščina revizijskih poročil SPO zdaj napajala prek UAL, podedovani revizijski signali pa so bili preseljeni v UAL.</span><span class="sxs-lookup"><span data-stu-id="51091-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="51091-116">Ključne spremembe:</span><span class="sxs-lookup"><span data-stu-id="51091-116">Key changes:</span></span>

- <span data-ttu-id="51091-117">Obrezovanje kot zmožnost ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="51091-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="51091-118">Odsek, v katerem izberete specifične dogodke za revizijo, ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="51091-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="51091-119">Prosimo, glejte [ta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) za popoln seznam revidiranih dogodkov, ki so privzeto na voljo.</span><span class="sxs-lookup"><span data-stu-id="51091-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="51091-120">Možnost» lokacija «v **poročilih po meri** ni na voljo.</span><span class="sxs-lookup"><span data-stu-id="51091-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="51091-121">Dogodki» odpiranje ali prenašanje dokumentov «niso na voljo.</span><span class="sxs-lookup"><span data-stu-id="51091-121">“Opening or downloading documents” events is NOT available.</span></span> 

