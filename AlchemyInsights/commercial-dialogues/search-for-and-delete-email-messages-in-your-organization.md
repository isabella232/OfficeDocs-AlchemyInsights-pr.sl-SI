---
title: Iskanje in brisanje e-poštnih sporočil v organizaciji
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750017"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="968e7-102">Iskanje in brisanje e-poštnih sporočil v organizaciji</span><span class="sxs-lookup"><span data-stu-id="968e7-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="968e7-103">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="968e7-103">Follow these steps:</span></span>

1. <span data-ttu-id="968e7-104">Če niste globalni skrbnik, morate poiskati sporočila, ki jih mora vaš račun dodati v **skupino vlog E-odkrivanje Manager** ali **upravljanje iskanja skladnosti**.</span><span class="sxs-lookup"><span data-stu-id="968e7-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="968e7-105">Če želite izbrisati sporočila, se morate vključiti v **skupino vlog za upravljanje organizacije** ali **vlogo za upravljanje iskanja in čiščenja**.</span><span class="sxs-lookup"><span data-stu-id="968e7-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="968e7-106">Dovoljenja za te vloge so dodeljena v [središču za skladnost varnostnega &.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="968e7-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="968e7-107">[Ustvarite iskanje vsebine](https://docs.microsoft.com/office365/securitycompliance/content-search) , da poiščete sporočilo, ki ga želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="968e7-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="968e7-108">[Vzpostavi povezavo z varnostnim središčem v središču za skladnost z varnostjo &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="968e7-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="968e7-109">Če uporabljate MFA, si oglejte ta navodila: [Povežite se s središčem za varnost & skladnost z uporabo multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="968e7-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="968e7-110">Izbrišite sporočilo: zaženite `New-ComplianceSearchAction` ukaz» cmdlet «, da izbrišete sporočilo.</span><span class="sxs-lookup"><span data-stu-id="968e7-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="968e7-111">Izbrisana sporočila so premaknjena v mapo» nadomestljive elemente uporabnika «.</span><span class="sxs-lookup"><span data-stu-id="968e7-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="968e7-112">Če želite ukaz» primer «, glejte [3. korak: izbrišite sporočilo.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="968e7-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
