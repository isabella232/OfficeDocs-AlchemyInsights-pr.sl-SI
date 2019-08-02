---
title: Potek dela email ni poslan
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059619"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="c66e9-102">Potek dela email ni poslan</span><span class="sxs-lookup"><span data-stu-id="c66e9-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="c66e9-103">Email s poteki dela se ne pošljejo vse uporabnike ali samo določenim uporabnikom, ali vidite napake **e-poštnega sporočila ni mogoče poslati. Preverite, ali je e-mail veljaven prejemnik**.</span><span class="sxs-lookup"><span data-stu-id="c66e9-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="c66e9-104">Preverite, če uporabnik obstaja v skupini **Vse ljudi** dovoljenja (seznam informacij uporabnik) za to zbirko mest.</span><span class="sxs-lookup"><span data-stu-id="c66e9-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="c66e9-105">Vzorec neposredno URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="c66e9-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="c66e9-106">Če uporabnik ne obstaja, se prepričajte, uporabnik je podpisal stran.</span><span class="sxs-lookup"><span data-stu-id="c66e9-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="c66e9-107">Če gre za zunanjega uporabnika, se prepričajte, da njihovo povabilo sprejme.</span><span class="sxs-lookup"><span data-stu-id="c66e9-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="c66e9-108">Če uporabnik obstaja v skupini dovoljenja, poskrbite, da naslov ni pravilen.</span><span class="sxs-lookup"><span data-stu-id="c66e9-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="c66e9-109">Če uporabniki e-poštni naslov ni nastavljena tukaj, ustvarite vzorec Opozorilo za tega uporabnika, ki sili sinhronizacijo uporabniški račun od uporabnikov profil SharePoint v tej zbirki mest.</span><span class="sxs-lookup"><span data-stu-id="c66e9-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="c66e9-110">Email s poteki dela pošiljajo skrbniki zbirke ne pa drugim uporabnikom in vidim napako \*\*HTTP prepovedano za <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="c66e9-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="c66e9-111">Glej [Dostop zavrnjen, ko sent email v skupine](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="c66e9-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="c66e9-112">Prav tako, preverite, ali funkcija zbirke mest **dostop omejen uporabnik dovoljenje lockdown način** ni aktivna.</span><span class="sxs-lookup"><span data-stu-id="c66e9-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="c66e9-113">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="c66e9-113">Related topics</span></span>
- [<span data-ttu-id="c66e9-114">Ustvari tok</span><span class="sxs-lookup"><span data-stu-id="c66e9-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c66e9-115">SharePoint in pretok</span><span class="sxs-lookup"><span data-stu-id="c66e9-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


