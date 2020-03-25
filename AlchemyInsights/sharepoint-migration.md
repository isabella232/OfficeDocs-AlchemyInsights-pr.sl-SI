---
title: Selitev možnosti v SharePoint online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932746"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="d81fa-102">Selitev možnosti v SharePoint online</span><span class="sxs-lookup"><span data-stu-id="d81fa-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="d81fa-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="d81fa-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d81fa-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="d81fa-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d81fa-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="d81fa-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d81fa-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="d81fa-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d81fa-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="d81fa-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d81fa-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="d81fa-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d81fa-109">**Možnosti selitve**</span><span class="sxs-lookup"><span data-stu-id="d81fa-109">**Migration options**</span></span>

<span data-ttu-id="d81fa-110">Za selitev vsebine v SharePoint online so na voljo različne možnosti, odvisno od velikosti in količine datotek, ki jih morate premakniti, si oglejte seznam možnosti, [ki se nahajajo tukaj](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="d81fa-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="d81fa-111">Več informacij o selitvi vsebine najdete v spodnjih povezavah.</span><span class="sxs-lookup"><span data-stu-id="d81fa-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="d81fa-112">SharePointovo orodje za selitev</span><span class="sxs-lookup"><span data-stu-id="d81fa-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="d81fa-113">Začnite z upraviteljem migracij</span><span class="sxs-lookup"><span data-stu-id="d81fa-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="d81fa-114">Hitrost selitve za SharePoint online in ODB</span><span class="sxs-lookup"><span data-stu-id="d81fa-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="d81fa-115">Izogibajte se temu, da bi v SharePoint online dobili ali blokirali</span><span class="sxs-lookup"><span data-stu-id="d81fa-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="d81fa-116">Orodje za ocenjevanje migracij v SharePointu (SMAT)</span><span class="sxs-lookup"><span data-stu-id="d81fa-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="d81fa-117">**Opomba**: trenutno orodje SharePoint Migration podpira samo selitev iz sharepointa 2010 in 2013.</span><span class="sxs-lookup"><span data-stu-id="d81fa-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="d81fa-118">Različica 2016 ali 2019 trenutno ni podprta.</span><span class="sxs-lookup"><span data-stu-id="d81fa-118">Version 2016 or 2019 are not supported at this time.</span></span>
