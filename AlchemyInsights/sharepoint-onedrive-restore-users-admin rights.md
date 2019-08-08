---
title: Odpravljanje težav dostop zavrnjen sporočila OneDrive za poslovne strani
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232557"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="329f3-102">Odpravljanje težav dostop zavrnjen sporočila OneDrive za poslovne strani</span><span class="sxs-lookup"><span data-stu-id="329f3-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="329f3-103">Težavo se najpogosteje pojavi, ko uporabnik izbriše in ponovno ustvari z enakim glavnim imenom uporabnika (UPN).</span><span class="sxs-lookup"><span data-stu-id="329f3-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="329f3-104">Novi račun je ustvarjen z uporabo različnih PUID (Passport Enolični ID) vrednost.</span><span class="sxs-lookup"><span data-stu-id="329f3-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="329f3-105">Ko uporabnik poskuša za dostop do zbirke mest ali njihovih OneDrive, uporabnik je napačno PUID.</span><span class="sxs-lookup"><span data-stu-id="329f3-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="329f3-106">Drugi scenarij vključuje sinhronizacija imenika z Active Directory organizacijska enota (OU).</span><span class="sxs-lookup"><span data-stu-id="329f3-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="329f3-107">Če uporabniki so že vpisani v SharePoint, in nato preselil v različnih OU in resynced s SharePointom, da lahko pride do te težave.</span><span class="sxs-lookup"><span data-stu-id="329f3-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="329f3-108">Če želite težavo odpraviti obnovite izvirno UPN s korakom v članku,[obnoviti uporabnik v Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="329f3-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="329f3-109">Če ne morete obnoviti izvirni uporabniki odstranite staro uporabnika s strani OneDrive, po teh korakih, [odstranite uporabnika iz seznamu informacij o uporabnikih]().</span><span class="sxs-lookup"><span data-stu-id="329f3-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="329f3-110">Ko je to storjeno, lahko preverite, ali ima uporabnik admin pravice do OneDrive mesta po navodilih za [Dodajanje admin je za uporabnika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="329f3-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="329f3-111">Več informacij na ravni dovoljenj, si oglejte članek, [razumevanje ravni dovoljenj v SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="329f3-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
