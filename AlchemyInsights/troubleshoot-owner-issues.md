---
title: Odpravljanje težav z lastnikom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901277"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="3a6b9-102">Odpravljanje težav z lastnikom</span><span class="sxs-lookup"><span data-stu-id="3a6b9-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="3a6b9-103">Če želite odpraviti težave z lastništvom, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="3a6b9-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="3a6b9-104">[Dodajte ali spremenite skrbnike naročnine na Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): skupine Azure Active Directory (Azure ad) so v lasti in jih upravljajo lastniki skupine.</span><span class="sxs-lookup"><span data-stu-id="3a6b9-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="3a6b9-105">Lastniki skupine so lahko uporabniki ali upravniki storitev in lahko upravljajo skupino, vključno s članstvom.</span><span class="sxs-lookup"><span data-stu-id="3a6b9-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="3a6b9-106">Lastnikom skupine lahko dodelite le obstoječe lastnike skupine ali skrbnike skupine.</span><span class="sxs-lookup"><span data-stu-id="3a6b9-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="3a6b9-107">Lastnikom skupine ni treba biti člani skupine.</span><span class="sxs-lookup"><span data-stu-id="3a6b9-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="3a6b9-108">[Dodajanje ali spreminjanje skrbnikov naročnine](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)na naročnino: v tem članku je opisano, kako dodate ali spremenite skrbniško vlogo za uporabnika s storitvijo Azure RBAC na obseg naročnin.</span><span class="sxs-lookup"><span data-stu-id="3a6b9-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="3a6b9-109">Uporabite PowerShell za dodajanje lastnika skupine ali lastnika aplikacije.</span><span class="sxs-lookup"><span data-stu-id="3a6b9-109">Use PowerShell to add a group owner or an application owner.</span></span>
