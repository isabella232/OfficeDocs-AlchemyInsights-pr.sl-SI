---
title: Nameščanje Officea v terminal server-brez licence
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508644"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="d5f0e-102">Nameščanje Officea v terminalski strežnik</span><span class="sxs-lookup"><span data-stu-id="d5f0e-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="d5f0e-103">Za uvajanje Microsoftovih 365 aplikacij za podjetje v operacijskem sistemu Windows Server z uporabo storitev oddaljenega namizja (RDS), prej imenovanih terminalske storitve:</span><span class="sxs-lookup"><span data-stu-id="d5f0e-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="d5f0e-104">Imeti morate naročnino na Microsoftovo 365, ki vključuje Microsoft 365 apps za podjetje, kot je Office 365 Enterprise E3 ali Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="d5f0e-105">Microsoft 365 Apps for Business in Microsoft 365 apps za poslovne Premium paketi ne vključujejo Microsoft 365 apps za podjetja.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="d5f0e-106">Omogočiti morate aktiviranje v [skupni rabi računalnika](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d5f0e-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="d5f0e-107">Če želite namestiti Microsoft 365 apps za podjetje na RDS iz Microsoft 365 skrbniško središče, ***ki uporablja privzete nastavitve namestitve***, uporabite naslednje korake.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="d5f0e-108">Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetje v načinu za aktiviranje v skupni rabi računalnika.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="d5f0e-109">Preverite, kaj Microsoft 365 naročnino imate.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="d5f0e-110">Preberite, kako</span><span class="sxs-lookup"><span data-stu-id="d5f0e-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="d5f0e-111">Če je potrebno, preklopite na drugo naročnino na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="d5f0e-112">Preberite, kako</span><span class="sxs-lookup"><span data-stu-id="d5f0e-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="d5f0e-113">Če je Office že nameščen v strežniku RDS z uporabo katere koli druge naročnine za Microsoft 365, ga odstranite.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="d5f0e-114">Na primer, z tekoč v pregled svet \> uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="d5f0e-115">Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="d5f0e-116">V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 apps za podjetje](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="d5f0e-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="d5f0e-117">Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="d5f0e-118">V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="d5f0e-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="d5f0e-119">Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite Zaženi.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="d5f0e-120">V polje Odpri vnesite **regedit**in nato izberite v redu.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="d5f0e-121">Izberite da, ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="d5f0e-122">V urejevalniku registra dodajte vrednost niza» **Sharedcomputerlicensing** «z nastavitvijo 1 pod HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d5f0e-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="d5f0e-123">V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Microsoft 365 apps za podjetje](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d5f0e-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="d5f0e-124">Če želite več podrobnosti o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje microsoftovih 365 aplikacij za podjetje z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d5f0e-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="d5f0e-125">Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi, si oglejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetje](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d5f0e-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  