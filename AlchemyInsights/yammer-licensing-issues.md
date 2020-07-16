---
title: Težave z izdajanjem licenc za yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148321"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="b0a8d-102">Težave z izdajanjem licenc za yammer</span><span class="sxs-lookup"><span data-stu-id="b0a8d-102">Yammer licensing issues</span></span>

<span data-ttu-id="b0a8d-103">Vsi uporabniki morajo imeti licenco za uporabo storitve Yammer Enterprise, vendar storitev Yammer privzeto ne zahteva, da imajo uporabniki licenco za dostop do storitve.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="b0a8d-104">Ko skrbnik spremeni nastavitev, da blokira Microsoft 365 uporabnike brez licenc Yammer, Uporabniki, ki niso dodelili licence Yammer Enterprise, ne morejo dostopati do storitve Yammer.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="b0a8d-105">Če želite več informacij, glejte [upravljanje uporabniških licenc za Yammer v Officeu 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="b0a8d-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="b0a8d-106">Ko so licence odstranjene iz uporabnikov, ploščica Yammer ni več prikazana, druge storitve pa lahko za skrivanje funkcij uporabljajo odstranjevanje licenc.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="b0a8d-107">V drugih primerih so funkcije še vedno lahko prikazane, vendar zahtevajo dodelitev licence za delovanje.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="b0a8d-108">**Licenca se ne posodablja za uporabnika**</span><span class="sxs-lookup"><span data-stu-id="b0a8d-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="b0a8d-109">Občasno je uporabniku dodeljena licenca, vendar še vedno ne more dostopati do Yammer.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="b0a8d-110">Zamude so verjetneje nastale, ko se izvaja dodelitev množične licence.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="b0a8d-111">Uporabniki storitev yammer morda ne bodo posodobljeni v enakem vrstnem redu, kot so licence spremenjene v storitvi Azure AD, ker sistem deluje asinhrono.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="b0a8d-112">Počakajte do 24 ur, preden odprete primer podpore za poročanje o težavah s sinhronizacijo licenc.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="b0a8d-113">**Dodelitev licence v velikem obsegu**</span><span class="sxs-lookup"><span data-stu-id="b0a8d-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="b0a8d-114">Licence lahko dodelite prek skrbniškega središča ali skriptov PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="b0a8d-115">Če želite več informacij, glejte [dodeljevanje licenc uporabnikom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) in [dodeljevanje licenc uporabniškim računom z Officeom 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="b0a8d-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="b0a8d-116">Microsoftova podpora ne zagotavlja pomoči pri ustvarjanju skriptov, vendar je na voljo dokumentacija o dodelitvi licenc za licenco Yammer.</span><span class="sxs-lookup"><span data-stu-id="b0a8d-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="b0a8d-117">Če želite več informacij, glejte [upravljanje licenc za Yammer z lupino Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="b0a8d-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>