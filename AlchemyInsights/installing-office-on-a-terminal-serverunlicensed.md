---
title: Nameščanje Officea v terminal server-brez licence
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735405"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="94900-102">Nameščanje Officea v terminalski strežnik</span><span class="sxs-lookup"><span data-stu-id="94900-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="94900-103">Zakaj napotitev urad 365 ProPlus naprej a okno pomočnik using zakoten pult usluga (RDS), prej imenovan semestralen usluga:</span><span class="sxs-lookup"><span data-stu-id="94900-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="94900-104">Imeti morate paket Office 365, ki vključuje Office 365 ProPlus, na primer Office 365 Enterprise E3 ali Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="94900-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="94900-105">Office 365 Business in Office 365 poslovni Premium načrti ne vključujejo Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="94900-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="94900-106">Omogočiti morate aktiviranje v [skupni rabi računalnika](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="94900-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="94900-107">Če želite namestiti Office 365 ProPlus na RDS iz Microsoft 365 skrbniškega centra, ***ki uporablja privzete nastavitve namestitve***, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="94900-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="94900-108">Preverite, kaj Office 365 načrt imate.</span><span class="sxs-lookup"><span data-stu-id="94900-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="94900-109">Preberite, kako</span><span class="sxs-lookup"><span data-stu-id="94900-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="94900-110">Če je potrebno, preklopite na drug paket Office 365.</span><span class="sxs-lookup"><span data-stu-id="94900-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="94900-111">Preberite, kako</span><span class="sxs-lookup"><span data-stu-id="94900-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="94900-112">Če je Office že nameščen v strežniku RDS z uporabo katerega koli drugega programa Office 365, ga odstranite.</span><span class="sxs-lookup"><span data-stu-id="94900-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="94900-113">Na primer, z tekoč v pregled svet \> uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu.</span><span class="sxs-lookup"><span data-stu-id="94900-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="94900-114">Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.</span><span class="sxs-lookup"><span data-stu-id="94900-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="94900-115">V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="94900-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="94900-116">Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.</span><span class="sxs-lookup"><span data-stu-id="94900-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="94900-117">V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="94900-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="94900-118">Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite Zaženi.</span><span class="sxs-lookup"><span data-stu-id="94900-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="94900-119">V polje Odpri vnesite **regedit**in nato izberite v redu.</span><span class="sxs-lookup"><span data-stu-id="94900-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="94900-120">Izberite da, ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.</span><span class="sxs-lookup"><span data-stu-id="94900-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="94900-121">V registracija urednik, povečati a tetiva vrednost od **Sharedcomputerlicensing** s a postavljanje od 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="94900-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="94900-122">V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="94900-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="94900-123">Če želite več podrobnosti o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje officea 365 ProPlus z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="94900-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="94900-124">Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi, glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="94900-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  