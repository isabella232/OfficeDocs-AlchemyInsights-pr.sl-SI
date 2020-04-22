---
title: ADFS Federation certifikat poteče
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710423"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="acc2f-102">ADFS Federation certifikat poteče</span><span class="sxs-lookup"><span data-stu-id="acc2f-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="acc2f-103">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="acc2f-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="acc2f-104">Namestite modul Microsoft Azure Active Directory za lupino Windows PowerShell v računalniku (če modul še ni nameščen).</span><span class="sxs-lookup"><span data-stu-id="acc2f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="acc2f-105">Če želite to narediti, pojdite na [upravljanje programa AZURE ad z lupino Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="acc2f-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="acc2f-106">Sledite korakom v razdelku» scenarij 1: potekla je veljavnost potrdila za podpisovanje žetonov AD FS «» [prišlo je do napake pri dostopu do mesta «iz programa AD FS, ko se je združil uporabnik v Microsoft 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="acc2f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="acc2f-107">Sledite korakom v [posodobitvi ali popravite nastavitve federativne domene v Microsoft, Azure ali InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="acc2f-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="acc2f-108">Če želite izvedeti več o podaljšanju potrdil federacije, glejte [obnovitev potrdil federacije za Microsoft 365 in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="acc2f-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
