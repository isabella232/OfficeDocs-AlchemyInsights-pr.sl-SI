---
title: Uvajanje dodatkov za Programi Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125686"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="e594f-102">Uvajanje dodatkov za Programi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e594f-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="e594f-103">Centralizirana uvedba je priporočen način uvedbe dodatkov Office uporabnikom in skupinam znotraj organizacije.</span><span class="sxs-lookup"><span data-stu-id="e594f-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="e594f-104">Če želite uvesti dodatke, upoštevajte spodnja navodila:</span><span class="sxs-lookup"><span data-stu-id="e594f-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="e594f-105">**Opomba:** Če želite namestiti dodatke za Office kot posamezen uporabnik, glejte Ogled, upravljanje in namestitev dodatkov [v Office programih.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="e594f-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="e594f-106">Poleg tega poskrbite, da Office omogočene individualne pridobitve dodatkov iz Trgovine.</span><span class="sxs-lookup"><span data-stu-id="e594f-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="e594f-107">Zagotovite, da vaše okolje izpolnjuje zahteve za uvedbo dodatkov s centralizirano uvedbo.</span><span class="sxs-lookup"><span data-stu-id="e594f-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="e594f-108">Če želite več informacij, glejte [Zahteve.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="e594f-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="e594f-109">Če želite **Nastavitve**  >  **dodatke,** si  >  **v** skrbniškem središču Microsoft 365 Office 2016 Microsoft 365 Pridobite aplikacije.</span><span class="sxs-lookup"><span data-stu-id="e594f-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="e594f-110">Opombe:</span><span class="sxs-lookup"><span data-stu-id="e594f-110">Notes:</span></span> 

- <span data-ttu-id="e594f-111">Integrirani programi zahtevajo, da ima skrbnik dovoljenja globalnega skrbnika Exchange skrbnika.</span><span class="sxs-lookup"><span data-stu-id="e594f-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="e594f-112">Ko uvajate dodatke za več uporabnikov, priporočamo, da za dodelitve uporabite skupine namesto posameznih uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="e594f-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="e594f-113">Če želite več [informacij, glejte Kaj je treba upoštevati pri dodeljevanju dodatka uporabnikom in skupinam.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="e594f-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="e594f-114">Centralizirana uvedba ne podpira uporabnikov v ugnezdenih skupinah ali skupinah, ki imajo nadrejene skupine.</span><span class="sxs-lookup"><span data-stu-id="e594f-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="e594f-115">Če želite več informacij, [glejte Dodelitve uporabnikov in skupin.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="e594f-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="e594f-116">Zagotovite, da je storitev za upravljanje Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogočena za uporabnike, da se vpišejo.</span><span class="sxs-lookup"><span data-stu-id="e594f-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="e594f-117">Če želite več informacij, [glejte Konfiguracija lastnosti aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="e594f-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="e594f-118">Če pride do težav pri uvajanju dodatkov z integriranimi programi, jih poskusite [uvesti z dodatki.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="e594f-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="e594f-119">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="e594f-119">For more information, see:</span></span>

<span data-ttu-id="e594f-120">[Uvajanje dodatkov v skrbniškem središču](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje dodatkov v skrbniškem središču](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Uporaba ukazov »cmdlet« PowerShell](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) za centralizirano uvedbo za upravljanje dodatkov 
 [Objavljanje Office dodatkov s centralizirano uvedbo prek skrbniškega središča Microsoft 365 za Office](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Odpravljanje težav: Uporabnik ne vidi dodatkov](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Odpravljanje napak uporabnikov Office dodatkov](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="e594f-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>