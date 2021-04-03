---
title: Obnovitev izbrisane skupine v storitvi Microsoft 365
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
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505707"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="45544-102">Obnovitev izbrisane skupine v storitvi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="45544-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="45544-103">Izbrisano skupino v storitvi Microsoft 365 ali Microsoft Teams lahko obnovite v 30 dneh od izbrisa.</span><span class="sxs-lookup"><span data-stu-id="45544-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="45544-104">Če se želite prijaviti v Skrbniško središče za Microsoft 365 in seznam izbrisanih skupin ter ekip, pojdite v [Skrbniško središče za Microsoft 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="45544-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="45544-105">**Opomba:** Prijavite se z računom, ki je dodeljen skrbniku najemnika ali skrbniški vlogi skupine.</span><span class="sxs-lookup"><span data-stu-id="45544-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="45544-106">Izberite izbrisano skupino/skupino Storitve Microsoft 365/Teams, ki jo želite obnoviti, in **kliknite obnovi skupino.**</span><span class="sxs-lookup"><span data-stu-id="45544-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="45544-107">Če skupine ni mogoče obnoviti zaradi naslova SMTP v sporu, uporabite ta ukaz, da najdete predmet, ki povzroča spor, in odstranite naslov SMTP:</span><span class="sxs-lookup"><span data-stu-id="45544-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="45544-108">**Opomba:** V nekaterih primerih lahko traja do 24 ur, da so skupina in vsi njeni podatki obnovljeni.</span><span class="sxs-lookup"><span data-stu-id="45544-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="45544-109">Če želite več informacij ali če želite izvedeti, kako obnovite skupine s storitvijo PowerShell, glejte Obnovitev izbrisane skupine v storitvi [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="45544-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>