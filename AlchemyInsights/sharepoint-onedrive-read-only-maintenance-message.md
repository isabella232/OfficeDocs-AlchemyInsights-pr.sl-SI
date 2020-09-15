---
title: Samo za branje za sporočilo o vzdrževanju pri poskusu uporabe SharePointa ali OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670848"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="6e242-102">Samo za branje za sporočilo o vzdrževanju pri poskusu uporabe SharePointa ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="6e242-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="6e242-103">Uporabniki lahko prejmejo sporočilo **za branje za vzdrževanje** , ko poskušajo uporabiti SharePoint ali OneDrive za enega od teh scenarijev.</span><span class="sxs-lookup"><span data-stu-id="6e242-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="6e242-104">Načrtovana ali aktivna vzdrževalna dejavnost.</span><span class="sxs-lookup"><span data-stu-id="6e242-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="6e242-105">Preverite jih tako, da se pomaknete do [središča za sporočila](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="6e242-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="6e242-106">Nepomemben dogodek, ki se lahko pojavi.</span><span class="sxs-lookup"><span data-stu-id="6e242-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="6e242-107">Preverite morebitne svetovalce/incidente tako, da se pomaknete na [stanje storitve](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6e242-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="6e242-108">Manjši postopek obnovitve samodejnega celjenja, ki se lahko zgodi zaradi morebitnih nepričakovanih dogodkov v strežnikih, ki bi lahko trajale manj kot 30 min.</span><span class="sxs-lookup"><span data-stu-id="6e242-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="6e242-109">Za te manjše okrevanje ni na voljo nobenega središča za sporočila ali mesta za zdravstveno stanje, vendar morate biti kmalu nazaj v normalno stanje.</span><span class="sxs-lookup"><span data-stu-id="6e242-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="6e242-110">V zelo redkih primerih smo opazili, da je bil eden od treh zgoraj navedenih primerov vzrok, storitev pa je bila obnovljena, vendar predpomnilnik brskalnika ni bil počiščen.</span><span class="sxs-lookup"><span data-stu-id="6e242-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="6e242-111">Poskusite počistiti predpomnilnik brskalnika, preden se pomaknete na mesto.</span><span class="sxs-lookup"><span data-stu-id="6e242-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="6e242-112">V brskalniku Microsoft Edge izberite **Nastavitve**in nato izberite **zasebnost in varnost**.</span><span class="sxs-lookup"><span data-stu-id="6e242-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="6e242-113">V razdelku **počistite brskanje**izberite **Izberite, kaj želite počistiti**.</span><span class="sxs-lookup"><span data-stu-id="6e242-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="6e242-114">Izberite **piškotke in shranjene podatke spletnega mesta**ter izberite **Počisti**.</span><span class="sxs-lookup"><span data-stu-id="6e242-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="6e242-115">Ti koraki se lahko razlikujejo, ko uporabljajo druge brskalnike, kot je Mozilla Firefox ali Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="6e242-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="6e242-116">Druga možnost je, da odprete SharePointovo mesto ali OneDrive v novem oknu InPrivate.</span><span class="sxs-lookup"><span data-stu-id="6e242-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>