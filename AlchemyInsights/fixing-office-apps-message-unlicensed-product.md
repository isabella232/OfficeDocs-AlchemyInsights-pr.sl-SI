---
title: Officea ni mogoče aktivirati
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812588"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="de7d4-102">Officea ni mogoče aktivirati</span><span class="sxs-lookup"><span data-stu-id="de7d4-102">Unable to activate Office</span></span>

- <span data-ttu-id="de7d4-103">Preverite, ali je stanje naročnine poteklo.</span><span class="sxs-lookup"><span data-stu-id="de7d4-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="de7d4-104">Prepričajte se, da imate naročnino, ki omogoča odjemalske licence, na primer Office 365 Business ali Business Premium in [se prepričajte, da je uporabniku dodeljena licenca](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="de7d4-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="de7d4-105">Prepričajte se, da se uporabnik vpisuje v Office z računom, za katerega je dodeljena licenca.</span><span class="sxs-lookup"><span data-stu-id="de7d4-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="de7d4-106">Oglejte si [stran z ustreznostjo stanja storitve Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) in preverite, ali obstajajo znane težave s storitvijo.</span><span class="sxs-lookup"><span data-stu-id="de7d4-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="de7d4-107">Preverite požarni zid, protivirusni program in nastavitve proxyja ter se prepričajte, da ne blokirajo dostopa Microsoft 365 aplikacij v internetu.</span><span class="sxs-lookup"><span data-stu-id="de7d4-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="de7d4-108">Glejte [URL-je in obsege naslovov IP za Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-ji in razponi naslovov IP za Office 365").</span><span class="sxs-lookup"><span data-stu-id="de7d4-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="de7d4-109">**Namig** na računalnikih s sistemom Windows lahko diagnosticirate in samodejno odpravite več pogostih težav pri vpisu v Office.</span><span class="sxs-lookup"><span data-stu-id="de7d4-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="de7d4-110">Prenesite in zaženite orodje **[Pomočnik za podporo in obnovitev](https://aka.ms/SaRA-OfficeSignInScenario)** za uporabo avtomatiziranega orodja.</span><span class="sxs-lookup"><span data-stu-id="de7d4-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="de7d4-111">Upoštevajte ta dejanja za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="de7d4-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="de7d4-112">Odprite Officeovo aplikacijo in se [izpišite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz obstoječega uporabniškega računa.</span><span class="sxs-lookup"><span data-stu-id="de7d4-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="de7d4-113">[Odstranite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) licenco za Office in jo [znova dodelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users), nato pa se [vpišite v Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) z uporabniškim računom, s katerim imate težave.</span><span class="sxs-lookup"><span data-stu-id="de7d4-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="de7d4-114">Zaženite [orodje za odpravljanje težav z aktiviranjem](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="de7d4-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="de7d4-115">Ponastavite stanje aktiviranja Officea</span><span class="sxs-lookup"><span data-stu-id="de7d4-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Ponastavite stanje aktiviranja Officea")
- [<span data-ttu-id="de7d4-116">Izvedite spletno popravilo Officea</span><span class="sxs-lookup"><span data-stu-id="de7d4-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="de7d4-117">Za dodatne rešitve odpravljanja težav glejte:</span><span class="sxs-lookup"><span data-stu-id="de7d4-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="de7d4-118">Napake v Officeu, povezane z nelicenciranim izdelkom in aktiviranjem</span><span class="sxs-lookup"><span data-stu-id="de7d4-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="de7d4-119">Pri aktiviranju Officea se prikaže napaka »Povezave z vašim računom ni mogoče vzpostaviti. Poskusite znova pozneje«</span><span class="sxs-lookup"><span data-stu-id="de7d4-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)