---
title: Eden od krajevnih certifikatov storitev federacije je potekel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785319"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="23d74-102">Eden od krajevnih certifikatov storitev federacije je potekel</span><span class="sxs-lookup"><span data-stu-id="23d74-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="23d74-103">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="23d74-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="23d74-104">Namestite modul Microsoft Azure Active Directory za lupino Windows PowerShell v računalniku (če modul še ni nameščen).</span><span class="sxs-lookup"><span data-stu-id="23d74-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="23d74-105">Če želite to narediti, pojdite na [lupino Azure Active Directory PowerShell za graf](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="23d74-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="23d74-106">Sledite korakom v razdelku» scenarij 1: potekla je veljavnost potrdila za podpisovanje žetonov AD FS «» [prišlo je do napake pri dostopu do mesta «iz programa AD FS, ko se je združil uporabnik v Microsoft 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="23d74-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="23d74-107">Sledite korakom, [Kako posodobiti ali popraviti nastavitve federirane domene v microsoftovih 365, Azure ali InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="23d74-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="23d74-108">Če želite več informacij o podaljšanju potrdil federacije, glejte [obnovitev certifikata za O365 in AZURE ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="23d74-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

