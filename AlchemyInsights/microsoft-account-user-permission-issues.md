---
title: Odpravljanje težav – uporabnik ni bil najden v imeniku
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754208"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="190a2-102">Odpravljanje težav – uporabnik ni bil najden v imeniku</span><span class="sxs-lookup"><span data-stu-id="190a2-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="190a2-103">Če uporabnik ste sprejemanje zmota vest "uporabnik vekanje ' obstati ustanavljati" v naslovnik.</span><span class="sxs-lookup"><span data-stu-id="190a2-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="190a2-104">Prosimo, poskusite znova, kjer je vrsta izdaje uporabnik ni v imeniku.</span><span class="sxs-lookup"><span data-stu-id="190a2-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="190a2-105">Za odpravljanje težave je mogoče dokončati naslednje korake.</span><span class="sxs-lookup"><span data-stu-id="190a2-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="190a2-106">Zagotovite, da je račun, ki je sprejel e-poštno povabilo, isti račun, ki se uporablja za vpis pozneje.</span><span class="sxs-lookup"><span data-stu-id="190a2-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="190a2-107">Prepričajte se, da uporabnik uporablja isti račun, da sprejme povabilo in se prijavite v spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="190a2-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="190a2-108">Če želite več informacij, glejte [kako upravljati vzdevke za svoj Microsoftov račun</a> , da upravljate Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="190a2-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="190a2-109">Prebrskajte do vsakega mesta (-ov), v katerem uporabnik prejema napako.</span><span class="sxs-lookup"><span data-stu-id="190a2-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="190a2-110">Dodaj "/_layouts/15/People.aspx/membershipgroupid = 0" (znotraj dvojnih narekovajev) do konca URL-ja spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="190a2-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="190a2-111">Primer: https://_ lt_ "contoso">. SharePoint. com/_ Layouts/15/ljudje. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="190a2-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="190a2-112">Izberite uporabnika s seznama.</span><span class="sxs-lookup"><span data-stu-id="190a2-112">Select the user from the list.</span></span>

- <span data-ttu-id="190a2-113">Kliknite **Odstrani uporabniške pravice** s traku.</span><span class="sxs-lookup"><span data-stu-id="190a2-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="190a2-114">Dodajte nazaj uporabnika in ponovno Pošlji povabilo uporabniku.</span><span class="sxs-lookup"><span data-stu-id="190a2-114">Add back the User and Resend the invite to the user.</span></span>

