---
title: Napeljati urad v terminalski strežnik - brez licence
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29490023"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="18e68-102">Namestite Office v terminalskem strežniku</span><span class="sxs-lookup"><span data-stu-id="18e68-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="18e68-103">Za uvajanje Office 365 ProPlus strežniku Windows z uporabo oddaljenega namizja storitve (RDS), prej imenovan terminalskih storitev:</span><span class="sxs-lookup"><span data-stu-id="18e68-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="18e68-p101">Morate imeti načrt Office 365, ki vključuje Office 365 ProPlus, kot so Office 365 podjetje E3 ali podjetje E5. Office 365 Business in Office 365 Business Premium načrti ne vključujejo Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="18e68-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="18e68-106">Morate omogočiti [skupno aktivacija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="18e68-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="18e68-107">Če želite namestiti Office 365 ProPlus na RDS na portalu Office 365, \*\* *ki uporablja privzeto nastavitev za namestitev* \*\*, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="18e68-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="18e68-p102">Ček kakšen načrt Office 365. [Izvedeti kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="18e68-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="18e68-p103">Če je potrebno, stikalo za različne Office 365 načrt. [Izvedeti kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="18e68-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="18e68-p104">Če je Office že nameščen na RDS strežnika z uporabo načrti za Office 365, ga odstranite. Na primer, z tekoč v pregled slika na lesu \> Uninstall program. Odstraniti z uporabo [Microsoft podporo in regres pomočnika](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če uporabljate problematike.</span><span class="sxs-lookup"><span data-stu-id="18e68-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="18e68-115">Na RDS strežnika, prijavite portalu Office 365 s skrbniškim računom in [namestite Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="18e68-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="18e68-116">Ko namestite Office, \*\* *ne odpreti ali znamenje v* \*\* za vse Officeove programe.</span><span class="sxs-lookup"><span data-stu-id="18e68-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="18e68-117">Na RDS strežnika, omogočiti aktiviranje porazdeliti računalo z urejanjem registra z naslednjim korakom:</span><span class="sxs-lookup"><span data-stu-id="18e68-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="18e68-p105">Z desno miškino tipko gumb Windows v spodnjem levem kotu zaslona in izberite Zaženi. V polje Odpri vnesite **regedit**in izberite OK.</span><span class="sxs-lookup"><span data-stu-id="18e68-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="18e68-120">Izbrati o čas sufler omogočiti registracija urednik narediti spremembe na napravi.</span><span class="sxs-lookup"><span data-stu-id="18e68-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="18e68-121">V registracija urednik, dodajte vrednost niza za **SharedComputerLicensing** z nastavitvijo 1 pod HKEY_LOCAL_MACHINESOFTWAREMicrosoft\ \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="18e68-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="18e68-122">V strežniku RDS \*\* *vpisati kot končnega uporabnika* \*\* in [Preverite, ali rabi aktivacija omogočen za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="18e68-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="18e68-123">Za več podrobnosti o pogoji, navodila za namestitev in navodila glede namestitve po meri z orodjem Office uvajanja, glejte [Uvajanje Office 365 ProPlus z uporabo storitve oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="18e68-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="18e68-124">Za odpravljanje napak, povezanih v skupni rabi activation, prosimo, glejte [Odpravljanje težav s skupno aktivacija za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="18e68-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

