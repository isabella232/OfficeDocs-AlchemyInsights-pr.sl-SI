---
title: E-pošta poteka dela ni poslana
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049389"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="c69f2-102">E-pošta poteka dela ni poslana za SharePointov seznam ali knjižnico</span><span class="sxs-lookup"><span data-stu-id="c69f2-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="c69f2-103">E-pošta iz potekov dela ni poslana vsem uporabnikom ali samo določenim uporabnikom ali pa se prikaže sporočilo o napaki, **da e-poštnega sporočila ni mogoče poslati. Preverite, ali ima e-pošta veljaven prejemnik**.</span><span class="sxs-lookup"><span data-stu-id="c69f2-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="c69f2-104">Preverite, ali uporabnik obstaja v skupini dovoljenja za **vse ljudi** (seznam uporabniških informacij) za to zbirko mest.</span><span class="sxs-lookup"><span data-stu-id="c69f2-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="c69f2-105">Sample neposredni URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="c69f2-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="c69f2-106">Če uporabnik ne obstaja, se prepričajte, da je uporabnik podpisan na strani.</span><span class="sxs-lookup"><span data-stu-id="c69f2-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="c69f2-107">Če je zunanji uporabnik, se prepričajte, da je bilo njihovo povabilo sprejeto.</span><span class="sxs-lookup"><span data-stu-id="c69f2-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="c69f2-108">Če uporabnik v skupini dovoljenj obstaja, se prepričajte, da je e-poštni naslov pravilen.</span><span class="sxs-lookup"><span data-stu-id="c69f2-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="c69f2-109">Če uporabnik e-poštni naslov ni nastavljen tukaj, nato pa ustvarite vzorčno Opozorilo za tega uporabnika, ki prisili sinhronizacijo tega uporabniškega računa iz uporabniških profilov SharePoint v to zbirko mest.</span><span class="sxs-lookup"><span data-stu-id="c69f2-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="c69f2-110">E-pošta iz potekov dela se pošlje skrbnikom zbirke mest, ne pa tudi drugim uporabnikom, in si oglejte napako **http prepovedano <span>https:</span>//URL/_vti_bin/Client.xvc.SP.utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="c69f2-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="c69f2-111">[Če pošljete e-poštno sporočilo v SharePointovo skupino, glejte dostop zavrnjen](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="c69f2-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="c69f2-112">Preverite tudi, ali je funkcija zbirke mest za **zaklepanje z omejenim dostopom uporabnika** neaktivna.</span><span class="sxs-lookup"><span data-stu-id="c69f2-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="c69f2-113">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="c69f2-113">Related topics</span></span>
<span data-ttu-id="c69f2-114">Želite poskusiti Microsoft Flow v SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="c69f2-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="c69f2-115">Ustvari potek</span><span class="sxs-lookup"><span data-stu-id="c69f2-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c69f2-116">SharePoint in Flow</span><span class="sxs-lookup"><span data-stu-id="c69f2-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


