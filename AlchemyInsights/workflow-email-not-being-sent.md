---
title: E-pošta poteka dela ni poslana
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749005"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="4a8a8-102">E-pošta poteka dela ni poslana za SharePointov seznam ali knjižnico</span><span class="sxs-lookup"><span data-stu-id="4a8a8-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="4a8a8-103">E-pošta iz potekov dela ni poslana vsem uporabnikom ali le določenim uporabnikom ali pa se prikaže sporočilo o napaki, da **e-poštnega sporočila ni mogoče poslati. Preverite, ali je e-pošta veljavna prejemnika**.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="4a8a8-104">Preverite, ali uporabnik obstaja v skupini dovoljenja za **vse osebe** (seznam uporabniških podatkov) za to zbirko mest.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="4a8a8-105">Vzorčni neposredni spletni naslov: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="4a8a8-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="4a8a8-106">Če uporabnik ne obstaja, se prepričajte, da je uporabnik vpisan na stran.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="4a8a8-107">Če gre za zunanjega uporabnika, se prepričajte, da je bilo njihovo povabilo sprejeto.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="4a8a8-108">Če uporabnik obstaja v skupini» dovoljenja «, se prepričajte, da je e-poštni naslov pravilen.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="4a8a8-109">Če e-poštni naslov za uporabnike ni nastavljen tukaj, ustvarite vzorčno Opozorilo za tega uporabnika, ki vsili sinhronizacijo tega uporabniškega računa iz uporabniških profilov SharePointa v to zbirko mest.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="4a8a8-110">E-pošta iz potekov dela je poslana skrbnikom zbirke mest, ne pa tudi drugim uporabnikom in si oglejte napako **http <span>:</span>//URL/_vti_bin/Client.xvc.SP.utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="4a8a8-111">[Če želite poslati e-poštno sporočilo v SharePointovo skupino, si oglejte dostop zavrnjen](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="4a8a8-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="4a8a8-112">Preverite tudi, ali funkcija zbirke mest z **omejenim dostopom za dovoljenje uporabnika** ni aktivna.</span><span class="sxs-lookup"><span data-stu-id="4a8a8-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="4a8a8-113">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="4a8a8-113">Related topics</span></span>
<span data-ttu-id="4a8a8-114">Ali želite preskusiti Microsoft Flow v storitvi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="4a8a8-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="4a8a8-115">Ustvarjanje toka</span><span class="sxs-lookup"><span data-stu-id="4a8a8-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="4a8a8-116">SharePoint in Flow</span><span class="sxs-lookup"><span data-stu-id="4a8a8-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


