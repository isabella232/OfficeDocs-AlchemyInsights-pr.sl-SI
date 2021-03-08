---
title: Nastavitev ClientAccessServerEnabled na True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525961"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="e9452-102">Nastavitev ClientAccessServerEnabled na True</span><span class="sxs-lookup"><span data-stu-id="e9452-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="e9452-103">Če ne morete odpreti šifriranega e-poštnega sporočila in namesto tega vidite Prilogo **rpmsg** , izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="e9452-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="e9452-104">Vzpostavite povezavo s storitvijo PowerShell Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e9452-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="e9452-105">Če želite vzpostaviti povezavo s storitvijo PowerShell Exchange Online, se morate vpisati s skrbniškim računom za globalni skrbnik ali Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9452-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="e9452-106">v.</span><span class="sxs-lookup"><span data-stu-id="e9452-106">a.</span></span> <span data-ttu-id="e9452-107">Odprite Windows PowerShell in zaženite ta ukaz: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="e9452-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="e9452-108">b.</span><span class="sxs-lookup"><span data-stu-id="e9452-108">b.</span></span> <span data-ttu-id="e9452-109">V pogovornem oknu **zahteva za poverilnice Windows PowerShell** vnesite službeni ali šolski račun in geslo, c.</span><span class="sxs-lookup"><span data-stu-id="e9452-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="e9452-110">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="e9452-110">Click **OK**.</span></span> 

2. <span data-ttu-id="e9452-111">Če želite ustvariti novo sejo, zaženite ta ukaz:</span><span class="sxs-lookup"><span data-stu-id="e9452-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="e9452-112">v.</span><span class="sxs-lookup"><span data-stu-id="e9452-112">a.</span></span> <span data-ttu-id="e9452-113">Zaženite ta ukaz:</span><span class="sxs-lookup"><span data-stu-id="e9452-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="e9452-114">`Get-IRMConfiguration`Ukaz» Zaženi «.</span><span class="sxs-lookup"><span data-stu-id="e9452-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="e9452-115">Preverite nastavitev **ClientAccessServerEnabled** .</span><span class="sxs-lookup"><span data-stu-id="e9452-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="e9452-116">v.</span><span class="sxs-lookup"><span data-stu-id="e9452-116">a.</span></span> <span data-ttu-id="e9452-117">Če je nastavitev **ClientAccessServerEnabled** nastavljena na» **FALSE**«, zaženite ta ukaz» cmdlet «: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="e9452-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="e9452-118">Vedno zaprite sejo lupine PowerShell s tem ukazom: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="e9452-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="e9452-119">Če želite več informacij, glejte [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="e9452-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

