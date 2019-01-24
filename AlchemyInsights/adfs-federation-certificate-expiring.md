---
title: ADF federacije potrdilo poteče
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29490130"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="60dba-102">ADF federacije potrdilo poteče</span><span class="sxs-lookup"><span data-stu-id="60dba-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="60dba-103">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="60dba-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="60dba-p101">Namestitev na Microsoft Azure Active Directory Module for Windows PowerShell v računalniku (če je modul ni že nameščen). Uganjati to, pojdite na [upravljanje Azure AD z lupino Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="60dba-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="60dba-106">Sledite korakom v je "scenarij 1: AD FS žeton podpisno potrdilo poteklo" oddelek [»Ni bilo problem dostop do strani« napaka iz AD FS, ko zunanji uporabnik prijavi v Office 365, Azure, ali Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="60dba-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="60dba-107">Sledite korakom kako [posodobite ali popravite nastavitve združeno domeno v Office 365, Azure, ali Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="60dba-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="60dba-108">Če želite izvedeti več o podaljšanju federacije potrdila, glej [Obnovi federacije potrdila za Office 365 in Azure storitve Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="60dba-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

