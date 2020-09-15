---
title: Uporabnikom omogočite dostop do SharePointa in OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677223"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="f9b13-102">Uporabnikom omogočite dostop do SharePointa in OneDrive</span><span class="sxs-lookup"><span data-stu-id="f9b13-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="f9b13-103">Če OneDrive ali SharePointovo mesto ni na voljo za več uporabnikov, ki so prej imeli dostop, je morda prišlo do začasne težave s storitvijo.</span><span class="sxs-lookup"><span data-stu-id="f9b13-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="f9b13-104">Preverjanje nadzorne plošče za stanje storitve</span><span class="sxs-lookup"><span data-stu-id="f9b13-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="f9b13-105">Če želite, da se osebe v organizaciji lahko vpišejo in uporabljajo SharePoint in OneDrive, morate zanje dodati račune in se prepričati, da imajo licenco, ki jim omogoča dostop do SharePointa in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f9b13-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="f9b13-106">Najpreprostejši način za dodajanje uporabnikov je v skrbniškem središču za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f9b13-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="f9b13-107">Pojdite na [stran aktivni uporabniki v skrbniškem središču za Microsoft 365](https://portal.office.com/adminportal/home#/users)in nato kliknite **Dodaj uporabnika**.</span><span class="sxs-lookup"><span data-stu-id="f9b13-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="f9b13-108">Vnesite informacije za uporabnika in se prepričajte, da je v razdelku **licence izdelka**dodeljena licenca in je izbrana možnost **SharePoint online** .</span><span class="sxs-lookup"><span data-stu-id="f9b13-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="f9b13-109">Če omogočite zunanjo skupno rabo v organizaciji, lahko uporabniki v organizaciji uporabljajo SharePoint in OneDrive vsebine z osebami zunaj organizacije.</span><span class="sxs-lookup"><span data-stu-id="f9b13-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="f9b13-110">Licenc zunanjih uporabnikov vam ni treba dati.</span><span class="sxs-lookup"><span data-stu-id="f9b13-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="f9b13-111">Poleg tega vam ni treba dodajati računov, razen če je skupna raba nastavljena na» le obstoječi zunanji uporabniki «.</span><span class="sxs-lookup"><span data-stu-id="f9b13-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="f9b13-112">Če v tem primeru ljudje niso v imeniku organizacije, jih morate dodati kot gostujoče uporabnike v skrbniškem središču za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9b13-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

