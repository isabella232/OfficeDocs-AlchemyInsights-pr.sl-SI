---
title: Selitev v SharePoint Online z upraviteljem selitve
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932372"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="69753-102">Selitev v SharePoint Online z upraviteljem selitve</span><span class="sxs-lookup"><span data-stu-id="69753-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="69753-103">**Pomembno**: veliko uporabnikov storitev SharePoint Online in OneDrive zaganjajo aplikacije, ključne za delovanje podjetja, v storitvi, ki se izvaja v ozadju.</span><span class="sxs-lookup"><span data-stu-id="69753-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="69753-104">Med te sodijo selitev vsebine, storitev preprečevanja izgube podatkov (DLP) in rešite za varnostno kopiranje.</span><span class="sxs-lookup"><span data-stu-id="69753-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="69753-105">Med temi nepredvidljivimi časi želimo poskrbeti, da storitvi SharePoint Online in OneDrive ostaneta razpoložljivi in zanesljivi za uporabnike, ki se bolj kot kdaj koli prej zanašajo na te storitve pri scenarijih oddaljenega dela.</span><span class="sxs-lookup"><span data-stu-id="69753-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="69753-106">Kot podporo temu cilju smo uvedli bolj stroge omejitve dušenja za aplikacije v ozadju (selitev, DLP in rešitve varnostnega kopiranja) med dnevnim časom delovnih dni.</span><span class="sxs-lookup"><span data-stu-id="69753-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="69753-107">Pričakujete lahko, da bo prepustnost teh aplikacij med tem obdobjem zelo nizka.</span><span class="sxs-lookup"><span data-stu-id="69753-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="69753-108">Toda med koncem tedna v regiji pa bo storitev pripravljena na obdelavo znatno večje količine zahtev aplikacij v ozadju.</span><span class="sxs-lookup"><span data-stu-id="69753-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="69753-109">**Upravitelj selitve**</span><span class="sxs-lookup"><span data-stu-id="69753-109">**Migration Manager**</span></span>

<span data-ttu-id="69753-110">Upravitelj selitve, ki je v sodobnem Skrbniškem središču SharePoint, vas vodi skozi postopek nastavitve odjemalcev in ustvarjanja opravil.</span><span class="sxs-lookup"><span data-stu-id="69753-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="69753-111">Določite lahko globalne nastavitve ali nastavitve na ravni opravila, si ogledate napredovanje opravila ter prenesete poročila s povzetkom ali poročila na ravni opravila.</span><span class="sxs-lookup"><span data-stu-id="69753-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="69753-112">Uvod v Upravitelja selitve</span><span class="sxs-lookup"><span data-stu-id="69753-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="69753-113">Nastavitev odjemalcev Upravitelja selitve</span><span class="sxs-lookup"><span data-stu-id="69753-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="69753-114">Nastavitve Upravitelja selitve</span><span class="sxs-lookup"><span data-stu-id="69753-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
