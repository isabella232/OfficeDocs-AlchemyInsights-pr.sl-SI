---
title: 932 nadgradnjo AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389766"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="26c6b-102">Nadgradnja sinje AD povezavo</span><span class="sxs-lookup"><span data-stu-id="26c6b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="26c6b-103">Privzeto samodejno nadgradnjo omogočena za Azure AD povezavo, ki pomaga zagotoviti, da uporabljate najnovejšo različico.</span><span class="sxs-lookup"><span data-stu-id="26c6b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="26c6b-104">Če želite preveriti samodejno nadgradnjo nastavitev, uporabite ukaz »cmdlet« **Get-ADSyncAutoUpgrade** v Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="26c6b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="26c6b-105">Ukaz »cmdlet «bo vrniti eno od naslednjih vrednosti:</span><span class="sxs-lookup"><span data-stu-id="26c6b-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="26c6b-106">**Omogočeno**: samodejno nadgradnjo omogočena.</span><span class="sxs-lookup"><span data-stu-id="26c6b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="26c6b-107">**Onemogočeno**: Samodejna nadgradnja onemogočena.</span><span class="sxs-lookup"><span data-stu-id="26c6b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="26c6b-108">**Pogojno**: sistem je ne več upravičeni do samodejne nadgradnje.</span><span class="sxs-lookup"><span data-stu-id="26c6b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="26c6b-109">Ne morete nastaviti te vrednosti; nastavljen sistem.</span><span class="sxs-lookup"><span data-stu-id="26c6b-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="26c6b-110">Če želite več informacij, glejte [samodejno nadgradnjo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="26c6b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="26c6b-111">Če želite prenesti najnovejšo različico Azure AD povezavo, pojdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="26c6b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
