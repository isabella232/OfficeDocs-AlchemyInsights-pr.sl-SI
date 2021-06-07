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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798696"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="a6acb-102">Officea ni mogoče aktivirati</span><span class="sxs-lookup"><span data-stu-id="a6acb-102">Unable to activate Office</span></span>

<span data-ttu-id="a6acb-103">**Opomba:** Če uporabljate starejšo različico programa Windows (na primer Windows 7), se prepričajte, da je TLS 1.2 omogočen kot privzeta različica.</span><span class="sxs-lookup"><span data-stu-id="a6acb-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="a6acb-104">Če želite več informacij, glejte Posodobitev, da omogočite [TLS 1.1 in TLS 1.2 kot](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)privzete varne protokole v winhttp v brskalniku Windows.</span><span class="sxs-lookup"><span data-stu-id="a6acb-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="a6acb-105">Preverite, ali je stanje naročnine poteklo.</span><span class="sxs-lookup"><span data-stu-id="a6acb-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="a6acb-106">Prepričajte se, da imate naročnino, ki omogoča odjemalske licence, na primer Office 365 Business ali Business Premium in [se prepričajte, da je uporabniku dodeljena licenca](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="a6acb-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="a6acb-107">Prepričajte se, da se uporabnik vpisuje v Office z računom, za katerega je dodeljena licenca.</span><span class="sxs-lookup"><span data-stu-id="a6acb-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="a6acb-108">Oglejte si [stran z ustreznostjo stanja storitve Office 365](/office365/enterprise/view-service-health) in preverite, ali obstajajo znane težave s storitvijo.</span><span class="sxs-lookup"><span data-stu-id="a6acb-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="a6acb-109">Preverite požarni zid, protivirusni program in nastavitve proxyja ter se prepričajte, da ne blokirajo dostopa Microsoft 365 aplikacij v internetu.</span><span class="sxs-lookup"><span data-stu-id="a6acb-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="a6acb-110">Glejte [URL-je in obsege naslovov IP za Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL-ji in razponi naslovov IP za Office 365").</span><span class="sxs-lookup"><span data-stu-id="a6acb-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="a6acb-111">**Namig** na računalnikih s sistemom Windows lahko diagnosticirate in samodejno odpravite več pogostih težav pri vpisu v Office.</span><span class="sxs-lookup"><span data-stu-id="a6acb-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="a6acb-112">Prenesite in zaženite orodje **[Pomočnik za podporo in obnovitev](https://aka.ms/SaRA-OfficeSignInScenario)** za uporabo avtomatiziranega orodja.</span><span class="sxs-lookup"><span data-stu-id="a6acb-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="a6acb-113">Upoštevajte ta dejanja za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="a6acb-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="a6acb-114">Odprite Officeovo aplikacijo in se [izpišite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz obstoječega uporabniškega računa.</span><span class="sxs-lookup"><span data-stu-id="a6acb-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="a6acb-115">[Odstranite](/microsoft-365/admin/manage/remove-licenses-from-users) licenco za Office in jo [znova dodelite](/microsoft-365/admin/manage/assign-licenses-to-users), nato pa se [vpišite v Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) z uporabniškim računom, s katerim imate težave.</span><span class="sxs-lookup"><span data-stu-id="a6acb-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="a6acb-116">Zaženite [orodje za odpravljanje težav z aktiviranjem](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="a6acb-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="a6acb-117">Ponastavite stanje aktiviranja Officea</span><span class="sxs-lookup"><span data-stu-id="a6acb-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Ponastavite stanje aktiviranja Officea")
- [<span data-ttu-id="a6acb-118">Izvedite spletno popravilo Officea</span><span class="sxs-lookup"><span data-stu-id="a6acb-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="a6acb-119">Za dodatne rešitve odpravljanja težav glejte:</span><span class="sxs-lookup"><span data-stu-id="a6acb-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="a6acb-120">Napake v Officeu, povezane z nelicenciranim izdelkom in aktiviranjem</span><span class="sxs-lookup"><span data-stu-id="a6acb-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="a6acb-121">Pri aktiviranju Officea se prikaže napaka »Povezave z vašim računom ni mogoče vzpostaviti. Poskusite znova pozneje«</span><span class="sxs-lookup"><span data-stu-id="a6acb-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)