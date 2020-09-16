---
title: Upravljanje sheme iskanja v storitvi SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770567"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="14e2b-102">Upravljanje sheme iskanja v storitvi SharePoint online</span><span class="sxs-lookup"><span data-stu-id="14e2b-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="14e2b-103">Shema iskanja nadzoruje, kateri uporabniki lahko iščejo, kako ga lahko uporabniki preiščejo in kako predstaviti rezultate na spletnih mestih iskanja.</span><span class="sxs-lookup"><span data-stu-id="14e2b-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="14e2b-104">Glejte [upravljanje sheme iskanja v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/manage-search-schema) , če želite izvedeti, kako:</span><span class="sxs-lookup"><span data-stu-id="14e2b-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="14e2b-105">Spremenite shemo iskanja.</span><span class="sxs-lookup"><span data-stu-id="14e2b-105">Change the search schema.</span></span>
- <span data-ttu-id="14e2b-106">Ustvarjanje upravljanih lastnosti.</span><span class="sxs-lookup"><span data-stu-id="14e2b-106">Create managed properties.</span></span>
- <span data-ttu-id="14e2b-107">Preiskane lastnosti preslikave map preiskane v upravljane lastnosti.</span><span class="sxs-lookup"><span data-stu-id="14e2b-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="14e2b-108">Zapomnite si to v zvezi z upravljanjem sheme iskanja:</span><span class="sxs-lookup"><span data-stu-id="14e2b-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="14e2b-109">Če prejmete opozorilo, ki navaja, **da je program začasno zaustavljen** , ko se spremeni shema, je to le začasno, saj je vzdrževanje storitve prisotno.</span><span class="sxs-lookup"><span data-stu-id="14e2b-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="14e2b-110">Če ste opravili več kot 24 ur in še vedno opazite opozorilo, se prijavite v primeru podpore.</span><span class="sxs-lookup"><span data-stu-id="14e2b-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="14e2b-111">Ko spremenite upravljane lastnosti ali dodate nove, začnejo spremembe veljati šele potem, ko je vsebina znova preiskana.</span><span class="sxs-lookup"><span data-stu-id="14e2b-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="14e2b-112">V storitvi SharePoint online se iskanje po vsebini samodejno zgodi na podlagi določenega načrta iskanja po vsebini.</span><span class="sxs-lookup"><span data-stu-id="14e2b-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="14e2b-113">Če se želite prepričati, da so vaše spremembe preiskane, lahko izrecno [zahtevate vnovično indeksiranje seznama ali knjižnice](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="14e2b-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="14e2b-114">Če želite dokončati pregled sheme iskanja, glejte [uvajanje sheme iskanja](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="14e2b-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


