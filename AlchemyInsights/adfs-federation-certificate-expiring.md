---
title: Potrdilo za povezovanje ADFS, ki poteče
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821967"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="7b5a2-102">Potrdilo za povezovanje ADFS, ki poteče</span><span class="sxs-lookup"><span data-stu-id="7b5a2-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="7b5a2-103">Če želite odpraviti to težavo, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="7b5a2-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="7b5a2-104">V računalnik namestite modul Microsoft Azure Active Directory za Windows PowerShell (če modul še ni nameščen).</span><span class="sxs-lookup"><span data-stu-id="7b5a2-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="7b5a2-105">Če želite to narediti, pojdite v [upravljanje imenika Azure AD z lupino Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="7b5a2-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="7b5a2-106">Upoštevajte navodila v razdelku »1. primer: Potrdilo za podpisovanje žetonov AD FS je poteklo« v razdelku »Pri storitvi AD FS je prišlo do težave pri dostopu do mesta«, ko se zvezni uporabnik prijavi v [Microsoft 365, Azure ali Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="7b5a2-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="7b5a2-107">Upoštevajte navodila v članku Posodobitev ali popravilo nastavitev domen v domeni [Microsoft, Azure ali Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="7b5a2-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="7b5a2-108">Če želite izvedeti več o podaljšanju potrdil za povezovanje, glejte [Podaljšanje potrdil združevanja za Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
