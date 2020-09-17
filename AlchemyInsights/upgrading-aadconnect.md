---
title: 932 nadgradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806055"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="45ec3-102">Nadgradnja povezave s storitvijo Azure AD</span><span class="sxs-lookup"><span data-stu-id="45ec3-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="45ec3-103">Samodejno nadgradnja je privzeto omogočena za povezavo s storitvijo Azure AD Connect, ki zagotavlja, da izvajate najnovejšo različico.</span><span class="sxs-lookup"><span data-stu-id="45ec3-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="45ec3-104">Če želite preveriti nastavitve samodejne nadgradnje, uporabite ukaz» cmdlet « **Get-ADSyncAutoUpgrade** v storitvi Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="45ec3-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="45ec3-105">Ukaz» cmdlet «bo vrnil eno od teh vrednosti:</span><span class="sxs-lookup"><span data-stu-id="45ec3-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="45ec3-106">**Omogočeno**: omogočena je Samodejna nadgradnja.</span><span class="sxs-lookup"><span data-stu-id="45ec3-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="45ec3-107">**Onemogočeno**: Samodejna nadgradnja je onemogočena.</span><span class="sxs-lookup"><span data-stu-id="45ec3-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="45ec3-108">**Začasno ustavljeno**: sistem ni več upravičen do samodejnega posodabljanja.</span><span class="sxs-lookup"><span data-stu-id="45ec3-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="45ec3-109">Te vrednosti ni mogoče konfigurirati; sistem je nastavljen s sistemom.</span><span class="sxs-lookup"><span data-stu-id="45ec3-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="45ec3-110">Če želite več informacij, glejte [Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="45ec3-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="45ec3-111">Če želite prenesti najnovejšo različico storitve Azure AD Connect, pojdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="45ec3-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
