---
title: Odpravljanje težav s sporočili o zavrnitvi dostopa
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051441"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="4c5b8-102">Odpravljanje težav pri dostopu zavrnjen v SharePoint/OneDrive skrbniško središče</span><span class="sxs-lookup"><span data-stu-id="4c5b8-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="4c5b8-103">Če prejmete sporočilo o zavrnitvi dostopa, ko poskušate prebrskati do skrbniškega središča SharePoint/OneDrive, se prepričajte, da [uporabniku dodelite licenco](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="4c5b8-104">Če ima uporabnik licenco, morate tudi poskrbeti, da jim je [dodeljena skrbniška vloga](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , ki lahko dostopa do skrbniških centrov.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="4c5b8-105">Ta težava se lahko pojavi tudi, ko je uporabnik izbrisan in ponovno ustvarjen z istim glavnim uporabniškim imenom (UPN).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4c5b8-106">Nov račun je ustvarjen z uporabo drugega PUID (Passport Enolični ID) vrednost.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4c5b8-107">Ko uporabnik poskuša dostopati do zbirke mest ali njihove storitve OneDrive, ima uporabnik napačen PUID.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4c5b8-108">Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4c5b8-109">Če so se uporabniki že prijavili v SharePoint, nato pa se premaknejo v drug OU in se znova sinhronizira s SharePointom, lahko to težavo izkusijo.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="4c5b8-110">Če želite odpraviti to težavo, obnovite izvirno UPN s koraki v članku, [obnovite uporabnika v Officeu 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="4c5b8-111">Opomba: Če v skrbniškem središču OneDrive ali SharePoint ni na voljo več uporabnikom, ki so že imeli dostop, lahko pride do začasne izdaje storitve.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="4c5b8-112">[Preverite nadzorno ploščo za zdravje storitve](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


