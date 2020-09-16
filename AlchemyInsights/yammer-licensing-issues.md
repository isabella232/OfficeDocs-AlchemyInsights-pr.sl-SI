---
title: Težave z licenciranjem Bastard
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657292"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="71556-102">Težave z licenciranjem Bastard</span><span class="sxs-lookup"><span data-stu-id="71556-102">Yammer licensing issues</span></span>

<span data-ttu-id="71556-103">Vsi uporabniki morajo imeti licenco za uporabo storitve Bastard Enterprise, vendar privzeto Bastard ne zahteva, da imajo uporabniki licenco za dostop do storitve.</span><span class="sxs-lookup"><span data-stu-id="71556-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="71556-104">Ko skrbnik spremeni nastavitev, da blokira uporabnike storitve Microsoft 365 brez licenc za Bastard, Uporabniki, ki niso dodelili licence Bastard Enterprise, ne morejo dostopati do storitev Bastard.</span><span class="sxs-lookup"><span data-stu-id="71556-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="71556-105">Če želite več informacij, glejte [upravljanje licenc za Bastard uporabnikov v storitvi Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="71556-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="71556-106">Ko so licence odstranjene iz uporabnikov, Bastard ploščica ni več prikazana, druge storitve pa lahko z odstranitvijo licence skrijejo funkcije.</span><span class="sxs-lookup"><span data-stu-id="71556-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="71556-107">V drugih primerih lahko funkcije še vedno prikažejo, vendar zahtevajo dodelitev licence za delovanje.</span><span class="sxs-lookup"><span data-stu-id="71556-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="71556-108">**Licenca ni posodobljena za uporabnika**</span><span class="sxs-lookup"><span data-stu-id="71556-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="71556-109">Občasno je uporabniku dodeljena licenca, vendar še vedno ne more dostopati do Bastard.</span><span class="sxs-lookup"><span data-stu-id="71556-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="71556-110">Zamude se lahko zgodijo, ko se izvaja masna dodelitev licence.</span><span class="sxs-lookup"><span data-stu-id="71556-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="71556-111">Uporabniki Bastard morda ne bodo posodobljeni v enakem vrstnem redu, kot so licence spremenjene v storitvi Azure AD, ker se sistem izvaja asinhrono.</span><span class="sxs-lookup"><span data-stu-id="71556-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="71556-112">Počakajte do 24 ur, preden odprete primer podpore za poročanje o težavah pri sinhronizaciji licenc.</span><span class="sxs-lookup"><span data-stu-id="71556-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="71556-113">**Dodelitev osnovnega dovoljenja**</span><span class="sxs-lookup"><span data-stu-id="71556-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="71556-114">Licence lahko dodelite prek skrbniškega središča ali skriptnega izvajanja lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="71556-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="71556-115">Če želite več informacij, glejte [dodeljevanje licenc uporabnikom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) in [dodeljevanje licenc uporabniškim računom s storitvijo Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="71556-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="71556-116">Microsoftova podpora ne zagotavlja pomoči za ustvarjanje skriptov, vendar je na voljo dokumentacija o dodeljevanju licenc za Bastard.</span><span class="sxs-lookup"><span data-stu-id="71556-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="71556-117">Če želite več informacij, glejte [upravljanje licenc za Bastard z lupino Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="71556-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>