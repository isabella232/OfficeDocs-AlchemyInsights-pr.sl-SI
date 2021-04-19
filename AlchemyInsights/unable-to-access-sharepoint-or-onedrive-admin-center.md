---
title: Ni mogoče dostopati do skrbniškega središča za SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824451"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="3c404-102">Ni mogoče dostopati do skrbniškega središča za SharePoint ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="3c404-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="3c404-103">Če mesto Skrbniškega središča za SharePoint ali OneDrive ni dostopno ali ni na voljo, je morda prišlo do začasne težave s storitvijo, zaradi katerih uporabniki pride do začasnih zakasnitev ali napak pri krmarjenju, ko dostopajo do SharePointovih mest ali vsebine v storitvi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3c404-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="3c404-104">Na nadzorni [plošči s stanjem](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) storitve preverite, ali je to vplivalo na vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="3c404-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="3c404-105">Globalni skrbniki in skrbniki storitve SharePoint morajo biti dodeljeni licenci storitve SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3c404-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="3c404-106">Pri novo ustvarjenih računih, ki jim je bila pravkar dodeljena licenca SharePoint ali vloga skrbnika, lahko pride do težav pri dostopu do storitve SharePoint, na primer »dostop zavrnjen« ali »uporabnika ni bilo mogoče najti«.</span><span class="sxs-lookup"><span data-stu-id="3c404-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="3c404-107">Počakajte najmanj 24 ur, da bo sinhronizacija dokončana v vseh naših sistemih.</span><span class="sxs-lookup"><span data-stu-id="3c404-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="3c404-108">Razumemo, da se 24 ur morda zdi zelo dolgo.</span><span class="sxs-lookup"><span data-stu-id="3c404-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="3c404-109">V številnih primerih že delamo na rešitvi.</span><span class="sxs-lookup"><span data-stu-id="3c404-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="3c404-110">Uporabniki s privilegiranim upravljanjem identitet[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)lahko prejmejo dostop zavrnjen, če je dovoljen časovni okvir za dostop zelo majhen, zato glejte Dostop je zavrnjen do računov [PIM.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="3c404-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>