---
title: Migracija omrežja
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: aada8e90d168a4c621dd81ee8d306b934c20d119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761830"
---
# <a name="network-migration"></a><span data-ttu-id="41b04-102">Migracija omrežja</span><span class="sxs-lookup"><span data-stu-id="41b04-102">Network Migration</span></span>

<span data-ttu-id="41b04-103">Vaš najemnik O365 je morda povezan z več omrežji Yammer v 1 najemniku: veliko omrežnih konfiguracij.</span><span class="sxs-lookup"><span data-stu-id="41b04-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="41b04-104">Začetek oktober 16, 2018, Yammer hoteti ne več zaslomba večkratnik Yammer omrežje združen s nedoločni zaimek najemnik.</span><span class="sxs-lookup"><span data-stu-id="41b04-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="41b04-105">Vi moči izvršiti nalogo a omrežje selitev zadobiti v a raje 1:1 zunanja podoba.</span><span class="sxs-lookup"><span data-stu-id="41b04-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="41b04-106">Če si želite ogledati seznam omrežij, povezanih z vašim najemnikom, se prijavite v storitev Yammer kot globalni skrbnik in prebrskajte do **omrežja admin**, nato pa **omrežno selitev**.</span><span class="sxs-lookup"><span data-stu-id="41b04-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="41b04-107">Izberite **naprej**.</span><span class="sxs-lookup"><span data-stu-id="41b04-107">Choose **Next**.</span></span>

- <span data-ttu-id="41b04-108">Če vidite več omrežij, naštetih v koraku 2 od 3, potem imate več omrežij Yammer, povezanih s svojim najemnikom O365.</span><span class="sxs-lookup"><span data-stu-id="41b04-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="41b04-109">Če želite popraviti konfiguracijo na 1:1 konfiguracijo, nadaljujte z orodjem za omrežno selitev.</span><span class="sxs-lookup"><span data-stu-id="41b04-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="41b04-110">Če želite več informacij o selitvi v omrežje, glejte [selitev omrežja: združite več omrežij Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="41b04-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="41b04-111">Prosimo, upoštevajte:</span><span class="sxs-lookup"><span data-stu-id="41b04-111">Please Note:</span></span>
  
- <span data-ttu-id="41b04-112">**Selitev omrežja seli samo aktivne in čakajoče uporabnike.**</span><span class="sxs-lookup"><span data-stu-id="41b04-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="41b04-113">Poleg aktivnih uporabnikov se preselite tudi informacije uporabnikov, kot sta ime in slika profila.</span><span class="sxs-lookup"><span data-stu-id="41b04-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="41b04-114">Vsa omrežna vsebina, vključno s skupinami, ni preseljena.</span><span class="sxs-lookup"><span data-stu-id="41b04-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="41b04-115">**Selitve omrežja ni mogoče razveljaviti.**</span><span class="sxs-lookup"><span data-stu-id="41b04-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="41b04-116">Po selitvi ne boste mogli dostopati do svojega odvisnega omrežja in njene vsebine.</span><span class="sxs-lookup"><span data-stu-id="41b04-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="41b04-117">Torej, preden Razmislite migracije, želite skrbno načrtovati.</span><span class="sxs-lookup"><span data-stu-id="41b04-117">So before you consider a migration, you want to plan carefully.</span></span>
