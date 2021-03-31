---
title: 126 Ali v programu OWA ni mogoče najti napake o nabiralniku?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426678"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="3f03f-102">Ali v Outlooku v spletu ni bilo mogoče najti napake nabiralnika?</span><span class="sxs-lookup"><span data-stu-id="3f03f-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="3f03f-103">Če uporabljate Outlook v spletu in  se prikaže sporočilo o napaki Nabiralnika ni bilo mogoče najti, račun, ki ste ga uporabili za povezovanje z Outlookom v spletu, nima licence za Exchange Online, zato z računom ni povezan noben nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="3f03f-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="3f03f-104">Vaš skrbnik lahko dodeli licenco računu tako, da upošteva te korake:</span><span class="sxs-lookup"><span data-stu-id="3f03f-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="3f03f-105">Odprite  [Skrbniško središče za Microsoft 365](https://portal.office.com/adminportal/home#/homepage)  in pojdite na Aktivni uporabniki v razdelku Uporabniki ter izberite uporabnika, ki vidi napako.</span><span class="sxs-lookup"><span data-stu-id="3f03f-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="3f03f-106">Na strani uporabnika, ki se  odpre, pojdite v razdelek  Licence in aplikacije, izberite ustrezno vrednost Lokacija in dodelite licenco, ki vsebuje Exchange Online (razširite licenco, da si ogledate njene podrobnosti).</span><span class="sxs-lookup"><span data-stu-id="3f03f-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="3f03f-107">Ko končate, kliknite **Shrani spremembe.**</span><span class="sxs-lookup"><span data-stu-id="3f03f-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="3f03f-108">Če je licenca v nekaterih primerih že dodeljena uporabniškem računu, lahko z odstranitvijo in ponovno dodelitevm licence odpravite težavo in jo pravilno uporabljate v sistemu:</span><span class="sxs-lookup"><span data-stu-id="3f03f-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="3f03f-109">Preverite, ali so vaše naročnine na M365 Exchange Online (in druge, če so na voljo) trenutne in še niso pred kratkim potekle.</span><span class="sxs-lookup"><span data-stu-id="3f03f-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="3f03f-110">Ko ste prepričani, da naročnina ni potekla in da je bila uporabniškeu računu dodeljena veljavna licenca, lahko traja do 24 ur, da je licenca omogočana, zato boste morali morda počakati, da se težava odpravi.</span><span class="sxs-lookup"><span data-stu-id="3f03f-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="3f03f-111">Če želite več informacij, [glejte Dodeljevanje in upravljanje licenc.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="3f03f-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>