---
title: SharePointova migracijska zadaviti s 503 napakami
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931674"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="9b5ea-102">SharePointova migracijska zadaviti s 503 napakami</span><span class="sxs-lookup"><span data-stu-id="9b5ea-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="9b5ea-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9b5ea-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9b5ea-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9b5ea-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9b5ea-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9b5ea-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9b5ea-109">**503 napake pri selitvi v SharePoint online**</span><span class="sxs-lookup"><span data-stu-id="9b5ea-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="9b5ea-110">Zdi se, da se preseljujejo v SharePoint online in prejemanje 503 napak.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="9b5ea-111">Prosimo, upoštevajte spodnja navodila, da vam lahko pomagamo v najkrajšem možnem času.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="9b5ea-112">Kliknite **Podpora za stik**in nato **Nova zahteva za storitev**.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="9b5ea-113">Za naslov in opis vnesite **SharePoint Migration Throttling z 503**.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="9b5ea-114">Ko je vozovnica oddana, jo posodobite z naslednjimi informacijami:</span><span class="sxs-lookup"><span data-stu-id="9b5ea-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="9b5ea-115">Koliko levo od migracije (na primer, koliko TBs?).</span><span class="sxs-lookup"><span data-stu-id="9b5ea-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="9b5ea-116">Začetek in končni datum selitve.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-116">Migration start and end date.</span></span>
    - <span data-ttu-id="9b5ea-117">Opišite, kje ste selitev vsebine iz, kot so SharePoint Server, Box, GDrive, datoteke delnice, itd.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="9b5ea-118">Ocenite število zadaviti napake (na primer, x dušenje na uro?) in kdaj je zadaviti zgodilo.</span><span class="sxs-lookup"><span data-stu-id="9b5ea-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="9b5ea-119">Katero orodje za selitev uporabljate (na primer SPMT ali ShareGate).</span><span class="sxs-lookup"><span data-stu-id="9b5ea-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


