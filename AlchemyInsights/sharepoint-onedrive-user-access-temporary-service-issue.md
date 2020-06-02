---
title: Težave z učinkovitostjo delovanja-SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511164"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ad530-102">SharePoint ali OneDrive počasen, nedostopen ali ni na voljo za več uporabnikov</span><span class="sxs-lookup"><span data-stu-id="ad530-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="ad530-103">Če OneDrive ali SharePointovo mesto ni na voljo več uporabnikom, ki so že imeli dostop, lahko pride do začasne izdaje storitve.</span><span class="sxs-lookup"><span data-stu-id="ad530-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="ad530-104">[Preverite nadzorno ploščo za zdravje storitve](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ad530-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ad530-105">**Dodajanje in licenciranje uporabnika**</span><span class="sxs-lookup"><span data-stu-id="ad530-105">**Add and license the user**</span></span>

<span data-ttu-id="ad530-106">Zagotovite, da boste [uporabnikom v Microsoftovem 365 za podjetja dodelili licence](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ad530-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="ad530-107">**Dodeljevanje dovoljenj**</span><span class="sxs-lookup"><span data-stu-id="ad530-107">**Assign Permissions**</span></span>

<span data-ttu-id="ad530-108">Če je bila uporabniku dodeljena licenca za SharePoint in še vedno prejema sporočilo o zavrnitvi dostopa, se prepričajte, da imajo dodeljeno [ustrezno raven dovoljenja](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="ad530-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="ad530-109">**Razmislite o uporabi funkcije zahteve za dostop**</span><span class="sxs-lookup"><span data-stu-id="ad530-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="ad530-110">[Funkcija zahteve za dostop](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ljudem omogoča, da zahtevajo dostop do vsebine, ki je trenutno nimajo dovoljenja za ogled.</span><span class="sxs-lookup"><span data-stu-id="ad530-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="ad530-111">**Dovoli skriptom po meri lahko povzroči težave pri dostopu**</span><span class="sxs-lookup"><span data-stu-id="ad530-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="ad530-112">Obstajajo določeni scenariji, v katerih lahko funkcija» *Dovoli skript po meri* «predstavlja dostop zavrnjen.</span><span class="sxs-lookup"><span data-stu-id="ad530-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="ad530-113">Zakaj a zapisati v seznam od zunanja oblika vplivati, varnost pomislek ter zmožnost v onesposobiti zunanja oblika.</span><span class="sxs-lookup"><span data-stu-id="ad530-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="ad530-114">Prosimo, obiščite [Dovoli ali prepreči skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="ad530-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

