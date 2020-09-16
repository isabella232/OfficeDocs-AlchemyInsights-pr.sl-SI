---
title: Težave z učinkovitostjo delovanja – SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771260"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4a4da-102">SharePoint ali OneDrive počasno, nedostopno ali ni na voljo za več uporabnikov</span><span class="sxs-lookup"><span data-stu-id="4a4da-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="4a4da-103">Če OneDrive ali SharePointovo mesto ni na voljo za več uporabnikov, ki so prej imeli dostop, je morda prišlo do začasne težave s storitvijo.</span><span class="sxs-lookup"><span data-stu-id="4a4da-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="4a4da-104">[Preverite nadzorno ploščo za stanje storitve](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4a4da-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="4a4da-105">**Dodajanje in licenciranje uporabnika**</span><span class="sxs-lookup"><span data-stu-id="4a4da-105">**Add and license the user**</span></span>

<span data-ttu-id="4a4da-106">Zagotovite, da [dodelite licence uporabnikom v storitvi Microsoft 365 za podjetja](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="4a4da-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="4a4da-107">**Dodeljevanje dovoljenj**</span><span class="sxs-lookup"><span data-stu-id="4a4da-107">**Assign Permissions**</span></span>

<span data-ttu-id="4a4da-108">Če je uporabniku dodeljena SharePointova licenca in še vedno prejema sporočilo o zavrnjenem dostopu, zagotovite, da je dodeljena [ustrezna raven dovoljenj](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="4a4da-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="4a4da-109">**Razmislite o uporabi funkcije zahteve za dostop**</span><span class="sxs-lookup"><span data-stu-id="4a4da-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="4a4da-110">[Funkcija zahteve za dostop](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) osebam omogoča, da zahtevajo dostop do vsebine, ki je trenutno nimajo dovoljenja za ogled.</span><span class="sxs-lookup"><span data-stu-id="4a4da-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="4a4da-111">**Dovoli skript po meri, lahko povzroči težave z zavrnjenim dostopom**</span><span class="sxs-lookup"><span data-stu-id="4a4da-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="4a4da-112">Obstajajo določeni scenariji, kjer lahko funkcija *skripta za dovolitev po meri* predstavlja dostop zavrnjen.</span><span class="sxs-lookup"><span data-stu-id="4a4da-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="4a4da-113">Seznam funkcij, ki so na voljo, varnostna opozorila in možnost onemogočanja funkcije.</span><span class="sxs-lookup"><span data-stu-id="4a4da-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="4a4da-114">Obiščite [Dovoli ali preprečite skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="4a4da-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

