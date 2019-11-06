---
title: 2609-zadržanje-ali-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994096"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="d609b-102">Elementov v storitvi SharePoint online ali OneDrive za podjetja ni mogoče izbrisati</span><span class="sxs-lookup"><span data-stu-id="d609b-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="d609b-103">Vi ali vaši uporabniki morda ne boste mogli izbrisati elementov v storitvi SharePoint online ali OneDrive za podjetja, ker je pravilnik o hranjenju, oznaki za hranjenje ali zadržanju za e-odkrivanje uporabljen na SharePointovem mestu OneDrive ali v določenem elementu.</span><span class="sxs-lookup"><span data-stu-id="d609b-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="d609b-104">To vključuje, da ne morete izbrisati dokumenta, različice dokumenta, mape, knjižnice dokumentov, seznama, aplikacije, mesta ali zbirke mest.</span><span class="sxs-lookup"><span data-stu-id="d609b-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="d609b-105">Tukaj je nekaj primerov sporočil o napakah, ki jih lahko prejmete, če poskušate izbrisati element, ki se obdrži:</span><span class="sxs-lookup"><span data-stu-id="d609b-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="d609b-106">» Tega spletnega mesta ni mogoče izbrisati, ker je vključen v pravilnik o zadržanju ali hranjenju e-odkrivanja «</span><span class="sxs-lookup"><span data-stu-id="d609b-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="d609b-107">"To položaj has a skladnost zvitost število enakih oseb v tnalo izbris"</span><span class="sxs-lookup"><span data-stu-id="d609b-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="d609b-108">"Politika skladnosti je trenutno blokira ta izbris strani"</span><span class="sxs-lookup"><span data-stu-id="d609b-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="d609b-109">"Te zbirke mest ni mogoče izbrisati, ker vsebuje mesta, ki so vključena v pravilnik o zadržanju ali hranjenju e-odkrivanja"</span><span class="sxs-lookup"><span data-stu-id="d609b-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="d609b-110">"Vi življati v izbrisati vsi reč v to zgibalnik spredaj vi izbrisati zgibalnik"</span><span class="sxs-lookup"><span data-stu-id="d609b-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="d609b-111">» Različic tega elementa ni mogoče izbrisati, ker je v pravilniku o zadržanju ali hranjenju «</span><span class="sxs-lookup"><span data-stu-id="d609b-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="d609b-112">» Elementa ni mogoče izbrisati med zadržkom «</span><span class="sxs-lookup"><span data-stu-id="d609b-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="d609b-113">» Oznaka, ki je uporabljena za ta element, preprečuje, da bi jo uredili ali izbrisali «</span><span class="sxs-lookup"><span data-stu-id="d609b-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="d609b-114">» Seznama ni mogoče izbrisati med zadržanjem ali pravilnikom o hranjenju «</span><span class="sxs-lookup"><span data-stu-id="d609b-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="d609b-115">"Seznama ni mogoče izbrisati, če je blokiran ali če se zanjo uporablja pravilnik o hranjenju."</span><span class="sxs-lookup"><span data-stu-id="d609b-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="d609b-116">Če želite izbrisati elemente v enem od teh scenarijev, je treba odstraniti pravilnik o hranjenju, oznako zadrževanja ali zadržanje e-odkrivanja (ali pa je mesto izključeno iz pravilnika o hranjenju).</span><span class="sxs-lookup"><span data-stu-id="d609b-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="d609b-117">Vi potreba v onesposobiti ali izključiti zadeven počakaj to ' causing to izdaja.</span><span class="sxs-lookup"><span data-stu-id="d609b-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="d609b-118">Ko je pravilnik o hranjenju ali zadržanje odstranjen, lahko traja do 24 ur, da sprememba učinkuje.</span><span class="sxs-lookup"><span data-stu-id="d609b-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="d609b-119">Če želite več informacij o različnih funkcijah hranjenja in zadržanja, ki jih je mogoče uporabiti na SharePointovih mestih in v računih storitve OneDrive, si oglejte eno od teh tem.</span><span class="sxs-lookup"><span data-stu-id="d609b-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="d609b-120">Pregled pravilnikov o hranjenju</span><span class="sxs-lookup"><span data-stu-id="d609b-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="d609b-121">Pregled oznak za hranjenje</span><span class="sxs-lookup"><span data-stu-id="d609b-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="d609b-122">Upravljanje zadržanj v naprednem e-odkrivanju</span><span class="sxs-lookup"><span data-stu-id="d609b-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="d609b-123">eDiscovery ima</span><span class="sxs-lookup"><span data-stu-id="d609b-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="d609b-124">Podedovane pravilnike o zaprtju in brisanju mest</span><span class="sxs-lookup"><span data-stu-id="d609b-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
