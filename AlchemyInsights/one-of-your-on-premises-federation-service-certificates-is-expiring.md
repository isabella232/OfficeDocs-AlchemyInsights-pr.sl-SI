---
title: Ena od vaših potrdil o storitvi federacije na mestu uporabe je potekla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673513"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="47d88-102">Ena od vaših potrdil o storitvi federacije na mestu uporabe je potekla</span><span class="sxs-lookup"><span data-stu-id="47d88-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="47d88-103">Če želite odpraviti to težavo, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="47d88-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="47d88-104">Namestite modul za Microsoft Azure Active Directory za Windows PowerShell v računalniku (če modul ni že nameščen).</span><span class="sxs-lookup"><span data-stu-id="47d88-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="47d88-105">To naredite tako, da se [poiščete v storitvi Azure Active Directory PowerShell za graf ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="47d88-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="47d88-106">Upoštevajte navodila v razdelku» scenarij 1: potrdilo o vpisu v strežnik AD FS je poteklo «v razdelku» [prišlo je do težave pri dostopu do mesta «v storitvi AD FS, ko se Združeno uporabnik prijavi v Microsoft 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="47d88-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="47d88-107">Upoštevajte navodila, [Kako posodobiti ali popraviti nastavitve Združenega domen v programu Microsoft 365, Azure ali InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="47d88-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="47d88-108">Če želite več informacij o obnovitvi potrdil federacije, si oglejte [podaljšanje potrdila za O365 in AZURE ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="47d88-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

