---
title: Splošna navodila za učinkovitost selitve
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932494"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="4b462-102">Splošna navodila za učinkovitost selitve</span><span class="sxs-lookup"><span data-stu-id="4b462-102">General migration performance guidance</span></span>

<span data-ttu-id="4b462-103">**Pomembno**: veliko uporabnikov storitev SharePoint Online in OneDrive zaganjajo aplikacije, ključne za delovanje podjetja, v storitvi, ki se izvaja v ozadju.</span><span class="sxs-lookup"><span data-stu-id="4b462-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4b462-104">Med te sodijo selitev vsebine, storitev preprečevanja izgube podatkov (DLP) in rešite za varnostno kopiranje.</span><span class="sxs-lookup"><span data-stu-id="4b462-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4b462-105">Med temi nepredvidljivimi časi želimo poskrbeti, da storitvi SharePoint Online in OneDrive ostaneta razpoložljivi in zanesljivi za uporabnike, ki se bolj kot kdaj koli prej zanašajo na te storitve pri scenarijih oddaljenega dela.</span><span class="sxs-lookup"><span data-stu-id="4b462-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4b462-106">Kot podporo temu cilju smo uvedli bolj stroge omejitve dušenja za aplikacije v ozadju (selitev, DLP in rešitve varnostnega kopiranja) med dnevnim časom delovnih dni.</span><span class="sxs-lookup"><span data-stu-id="4b462-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4b462-107">Pričakujete lahko, da bo prepustnost teh aplikacij med tem obdobjem zelo nizka.</span><span class="sxs-lookup"><span data-stu-id="4b462-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4b462-108">Toda med koncem tedna v regiji pa bo storitev pripravljena na obdelavo znatno večje količine zahtev aplikacij v ozadju.</span><span class="sxs-lookup"><span data-stu-id="4b462-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4b462-109">**Navodila za učinkovito selitev**</span><span class="sxs-lookup"><span data-stu-id="4b462-109">**Migration performance guidance**</span></span>

<span data-ttu-id="4b462-110">Na učinkovitost selitve lahko vpliva infrastruktura omrežja, velikost datoteke, čas selitve in omejevanje zmogljivosti.</span><span class="sxs-lookup"><span data-stu-id="4b462-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="4b462-111">Če boste imeli več informacij o teh dejavnikih, boste lahko bolje načrtovali in povečali učinkovitost selitve.</span><span class="sxs-lookup"><span data-stu-id="4b462-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="4b462-112">Splošna navodila za učinkovito selitev</span><span class="sxs-lookup"><span data-stu-id="4b462-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
