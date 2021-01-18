---
title: Težave s pridružitvijo VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885661"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="3bbcd-102">Težave s pridružitvijo VMs</span><span class="sxs-lookup"><span data-stu-id="3bbcd-102">Issue joining VMs</span></span>

<span data-ttu-id="3bbcd-103">Če želite odpraviti težave, ki se pojavijo med poskusom združevanja VMs, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="3bbcd-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="3bbcd-104">Poskusite se vpisati z obliko **UPN** (na primer» joeuser@contoso.com «), namesto v obliki zapisa **SAMAccountName** (» CONTOSO\joeuser «).</span><span class="sxs-lookup"><span data-stu-id="3bbcd-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="3bbcd-105">Zagotovite, da ste omogočili sinhronizacijo gesel v skladu z navodili, opisanimi v vodniku *za uvod.*</span><span class="sxs-lookup"><span data-stu-id="3bbcd-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="3bbcd-106">Zagotovite, da prizadeti uporabniški račun ni zunanji račun v storitvi Azure AD najemnik.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="3bbcd-107">Zunanji uporabniki se ne morejo vpisati v upravljano domeno, saj storitve Azure AD Domain Services nimajo poverilnic za te uporabniške račune.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="3bbcd-108">Če je prizadeti uporabniški račun le uporabniški račun v oblaku, zagotovite, da so uporabniki spremenili svoje geslo, potem ko ste omogočili domenske storitve Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="3bbcd-109">Ta korak povzroči, da so vrednosti za poverilnice, ki jih potrebujete za storitev Azure AD Domain, ustvarjene.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="3bbcd-110">Če so prizadeti uporabniški računi sinhronizirani iz imenika na mestu uporabe, preverite, ali je bila priporočena izdaja storitve Azure AD Connect konfigurirana tako, da izvaja popolno sinhronizacijo.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="3bbcd-111">Če težave ne morete odpraviti po potrditvi koraka 4, izvedite te ukaze iz sinhronizacijskega računalnika:</span><span class="sxs-lookup"><span data-stu-id="3bbcd-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="3bbcd-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="3bbcd-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>