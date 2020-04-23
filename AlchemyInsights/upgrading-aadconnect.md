---
title: 932 nadgradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766509"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="f3b82-102">Nadgradnja povezave Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f3b82-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="f3b82-103">Samodejna nadgradnja je privzeto omogočena za Azure AD Connect, ki pomaga zagotoviti, da uporabljate najnovejšo različico.</span><span class="sxs-lookup"><span data-stu-id="f3b82-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="f3b82-104">Če želite preveriti samodejne nastavitve nadgradnje, uporabite ukaz» cmdlet « **Get-ADSyncAutoUpgrade** v POWERSHELL Azure ad.</span><span class="sxs-lookup"><span data-stu-id="f3b82-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="f3b82-105">Ukaz» cmdlet «bo vrnil eno od naslednjih vrednosti:</span><span class="sxs-lookup"><span data-stu-id="f3b82-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="f3b82-106">**Omogočeno**: Samodejna nadgradnja je omogočena.</span><span class="sxs-lookup"><span data-stu-id="f3b82-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="f3b82-107">**Onemogočeno**: Samodejna nadgradnja je onemogočena.</span><span class="sxs-lookup"><span data-stu-id="f3b82-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="f3b82-108">**Prekinjena**: sistem ni več upravičen do samodejnega nadgrajevanja.</span><span class="sxs-lookup"><span data-stu-id="f3b82-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="f3b82-109">Te vrednosti ni mogoče konfigurirati; je nastavljen s sistemom.</span><span class="sxs-lookup"><span data-stu-id="f3b82-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="f3b82-110">Če želite več informacij, glejte [Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="f3b82-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="f3b82-111">Če želite prenesti najnovejšo različico Azure AD Connect, pojdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="f3b82-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
