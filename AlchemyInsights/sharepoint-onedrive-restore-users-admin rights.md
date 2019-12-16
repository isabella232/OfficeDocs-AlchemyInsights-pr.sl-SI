---
title: Odpravljanje težav pri dostopu zavrnjen sporočila na spletna mesta OneDrive za podjetja
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051621"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="4b61d-102">Odpravljanje težav pri dostopu zavrnjen sporočila na spletna mesta OneDrive za podjetja</span><span class="sxs-lookup"><span data-stu-id="4b61d-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="4b61d-103">Ta težava se najpogosteje pojavi, ko je uporabnik izbrisan in ponovno ustvarjen z istim glavnim imenom uporabnika (UPN).</span><span class="sxs-lookup"><span data-stu-id="4b61d-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="4b61d-104">Nov račun je ustvarjen z uporabo drugega PUID (Passport Enolični ID) vrednost.</span><span class="sxs-lookup"><span data-stu-id="4b61d-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="4b61d-105">Ko uporabnik poskuša dostopati do zbirke mest ali njihove storitve OneDrive, ima uporabnik napačen PUID.</span><span class="sxs-lookup"><span data-stu-id="4b61d-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="4b61d-106">Drugi scenarij vključuje sinhronizacijo imenika z organizacijsko enoto Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="4b61d-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="4b61d-107">Če so se uporabniki že prijavili v SharePoint, nato pa se premaknejo v drug OU in se znova sinhronizira s SharePointom, lahko to težavo izkusijo.</span><span class="sxs-lookup"><span data-stu-id="4b61d-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="4b61d-108">Če želite odpraviti to težavo, morate obnoviti izvirni UPN s koraki v članku, [obnovite uporabnika v Officeu 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4b61d-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="4b61d-109">Če prvotnega uporabnika ne morete obnoviti, odstranite starega uporabnika s spletnega mesta OneDrive s temi koraki, [odstranite uporabnika s seznama uporabniških podatkov]().</span><span class="sxs-lookup"><span data-stu-id="4b61d-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="4b61d-110">Ko je to storjeno, lahko preverite, ali ima uporabnik skrbniške pravice do mesta OneDrive, tako da sledi korakom, da [dodate skrbnika za uporabnikovo storitev onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="4b61d-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="4b61d-111">Če želite več informacij o ravneh dovoljenj, si oglejte članek, [razumevanje ravni dovoljenj v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4b61d-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
