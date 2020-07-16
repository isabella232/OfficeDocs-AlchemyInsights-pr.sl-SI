---
title: Izdaja odpiranja ali prenosa datotek v storitvi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148341"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="64ee0-102">Izdaja odpiranja ali prenosa datotek v storitvi Yammer</span><span class="sxs-lookup"><span data-stu-id="64ee0-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="64ee0-103">Classic Yammer podpira več možnosti za nalaganje datotek v sporočila in skupine.</span><span class="sxs-lookup"><span data-stu-id="64ee0-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="64ee0-104">Glede na konfiguracijo omrežja so datoteke privzete za shranjevanje v SharePointu.</span><span class="sxs-lookup"><span data-stu-id="64ee0-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="64ee0-105">Izbirnik datotek v novi storitvi Yammer še ne podpira vseh možnosti, ki so na voljo v klasični storitvi Yammer.</span><span class="sxs-lookup"><span data-stu-id="64ee0-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="64ee0-106">Prihodnja posodobitev bo dodala dodatne funkcije.</span><span class="sxs-lookup"><span data-stu-id="64ee0-106">A future update will add additional features.</span></span> <span data-ttu-id="64ee0-107">Če želite več informacij, glejte [prilaganje datoteke ali slike v mesto pogovora v storitvi Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="64ee0-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="64ee0-108">**Datoteke ni mogoče odpreti ali prenesti**</span><span class="sxs-lookup"><span data-stu-id="64ee0-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="64ee0-109">Datoteka se lahko naloži v storitev Yammer, vendar se poveže tudi z datoteko v storitvi SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="64ee0-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="64ee0-110">Če želite odpraviti težave, morate najprej določiti lokacijo datoteke.</span><span class="sxs-lookup"><span data-stu-id="64ee0-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="64ee0-111">Če je bila datoteka naložena v storitev Yammer, bo imela URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="64ee0-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="64ee0-112">Zagotovite, da so zahtevani URL-ji in naslovi IP neblokirani.</span><span class="sxs-lookup"><span data-stu-id="64ee0-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="64ee0-113">Če želite več informacij, glejte objavo v spletnem dnevniku [z uporabo trdih kodiranih IP naslovov za Yammer ni priporočljiva](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="64ee0-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="64ee0-114">Preverite, ali lahko uporabnik, ki je tudi globalni skrbnik, prenese datoteko.</span><span class="sxs-lookup"><span data-stu-id="64ee0-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="64ee0-115">Če je datoteka zasebna, boste morda morali uporabiti način zasebnega vsebine.</span><span class="sxs-lookup"><span data-stu-id="64ee0-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="64ee0-116">Če želite več informacij, glejte [spremljanje zasebne vsebine v storitvi Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="64ee0-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="64ee0-117">**Gosti in datoteke na ravni omrežja yammer v storitvi SharePoint online**</span><span class="sxs-lookup"><span data-stu-id="64ee0-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="64ee0-118">[Gosti na ravni omrežja v storitvi Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne uporabljajo storitve AZURE ad B2B in so notranji v storitvi yammer, zato ne morejo dostopati do datotek yammer, shranjenih v SharePointu.</span><span class="sxs-lookup"><span data-stu-id="64ee0-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="64ee0-119">Ustvarite zunanjega uporabnika AAD B2B, ki lahko dostopa do knjižnic dokumentov v SharePoint online z uporabo te identitete.</span><span class="sxs-lookup"><span data-stu-id="64ee0-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="64ee0-120">Če želite več informacij o prihodnji podpori za gostjo Azure AD B2B v storitvi Yammer, si oglejte [podporo za podjetja v storitvi Yammer preview – pogoji za stranke in pogosta vprašanja](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="64ee0-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>