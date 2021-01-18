---
title: Dodeljevanje skupin v vlogo Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885398"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="4b398-102">Dodeljevanje skupin v vlogo Azure AD</span><span class="sxs-lookup"><span data-stu-id="4b398-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="4b398-103">Če želite dodeliti skupino oglasov Azure ad z izvorom avtoritete v storitvi Azure AD na vlogo v storitvi Azure AD, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="4b398-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="4b398-104">Ustvarjanje nove skupine – če želite ustvariti novo skupino:</span><span class="sxs-lookup"><span data-stu-id="4b398-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="4b398-105">v.</span><span class="sxs-lookup"><span data-stu-id="4b398-105">a.</span></span> <span data-ttu-id="4b398-106">Vpišite se v skrbniško središče za Azure AD s **privilegiranim skrbnikom za vloge** ali **globalnimi skrbniškimi** dovoljenji.</span><span class="sxs-lookup"><span data-stu-id="4b398-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="4b398-107">b.</span><span class="sxs-lookup"><span data-stu-id="4b398-107">b.</span></span> <span data-ttu-id="4b398-108">Izberite **Azure Active Directory > skupine > vse skupine > novo skupino**.</span><span class="sxs-lookup"><span data-stu-id="4b398-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="4b398-109">c.</span><span class="sxs-lookup"><span data-stu-id="4b398-109">c.</span></span> <span data-ttu-id="4b398-110">Ustvarite skupino.</span><span class="sxs-lookup"><span data-stu-id="4b398-110">Create the group.</span></span>

2. <span data-ttu-id="4b398-111">Dodelite vlogo skupini bodisi med ustvarjanjem skupine ali ko je skupina ustvarjena.</span><span class="sxs-lookup"><span data-stu-id="4b398-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="4b398-112">v.</span><span class="sxs-lookup"><span data-stu-id="4b398-112">a.</span></span> <span data-ttu-id="4b398-113">Če želite skupini dodeliti vlogo v času ustvarjanja skupine, lahko v skupino dodelite vloge preklopnega programa **AZURE ad** in ustvarite skupino.</span><span class="sxs-lookup"><span data-stu-id="4b398-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="4b398-114">b.</span><span class="sxs-lookup"><span data-stu-id="4b398-114">b.</span></span> <span data-ttu-id="4b398-115">Če želite skupini dodeliti vlogo, ko je bila ustvarjena, se pomaknite do zavihka **dodeljene vloge** za novo ustvarjeno skupino in dodelite vlogo skupini.</span><span class="sxs-lookup"><span data-stu-id="4b398-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="4b398-116">**Upravljanje članstva v skupini, ki je dodeljena vlogi storitve Azure AD**</span><span class="sxs-lookup"><span data-stu-id="4b398-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="4b398-117">Če želite preprečiti dviganje privilegijev, lahko privzeti skrbniki, ki so dodeljeni vlogi, spremenijo le privilegirane skrbnike vlog in globalni skrbniki.</span><span class="sxs-lookup"><span data-stu-id="4b398-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="4b398-118">Lahko pa se odločijo, da bodo dodeljene lastniku za to skupino in da prenesejo to opravilo.</span><span class="sxs-lookup"><span data-stu-id="4b398-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="4b398-119">Če želite več podrobnosti o dodeljevanju skupin v oblaku za vloge v storitvi Azure AD, [si oglejte Dodeljevanje vlog v skupini Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="4b398-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="4b398-120">Če želite več informacij o odpravljanju težav, dodeljenih skupinam v oblaku, glejte [Odpravljanje težav z vlogami, dodeljenimi skupinam v oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="4b398-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





