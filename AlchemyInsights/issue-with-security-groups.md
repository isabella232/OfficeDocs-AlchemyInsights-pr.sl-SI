---
title: Težava z varnostnimi skupinami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177633"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="fa2dd-102">Težava z varnostnimi skupinami</span><span class="sxs-lookup"><span data-stu-id="fa2dd-102">Issue with security groups</span></span>

<span data-ttu-id="fa2dd-103">**Če prihaja do napake v omrežju AADDS104**</span><span class="sxs-lookup"><span data-stu-id="fa2dd-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="fa2dd-104">Neveljavna pravila skupine za varnost omrežja so najpogostejši vzrok za napake omrežja za domenske storitve Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="fa2dd-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="fa2dd-105">Skupina za varnost omrežja za navidezno omrežje mora omogočati dostop do določenih vrat in protokolov.</span><span class="sxs-lookup"><span data-stu-id="fa2dd-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="fa2dd-106">Če so ta vrata blokirana, platforma Azure ne more nadzorovati ali posodobiti upravljane domene.</span><span class="sxs-lookup"><span data-stu-id="fa2dd-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="fa2dd-107">Vpliva tudi sinhronizacija med storitvijo Azure AD in Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="fa2dd-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="fa2dd-108">Zagotovite, da so privzeta vrata odprta, da se izognete prekinitvi v storitvi.</span><span class="sxs-lookup"><span data-stu-id="fa2dd-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="fa2dd-109">Če želite razumeti in razrešiti pogosta opozorila za težave s konfiguracijo omrežja za varnost, glejte [Dodajanje in preverjanje varnostnih skupin](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="fa2dd-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
