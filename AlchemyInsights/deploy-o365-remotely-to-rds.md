---
title: Uvajanje Officea 365 ProPlus za skupno uporabo na RDS, terminalskem strežniku ali VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959475"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="89e1b-102">Uvajanje Officea 365 ProPlus za skupno uporabo na RDS, terminalskem strežniku ali VDI</span><span class="sxs-lookup"><span data-stu-id="89e1b-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="89e1b-103">Če želite uvesti Office 365 ProPlus z uporabo storitev oddaljenega namizja (RDS), prej imenovane terminalske storitve:</span><span class="sxs-lookup"><span data-stu-id="89e1b-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="89e1b-104">Imeti morate Microsoft 365 za poslovni načrt ali paket Office 365, ki vključuje Office 365 ProPlus, kot je Office 365 Enterprise E3 ali Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="89e1b-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="89e1b-105">Office 365 Business in Office 365 poslovni Premium načrti ne vključujejo Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="89e1b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="89e1b-106">Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="89e1b-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="89e1b-107">Vi moči tudi travnato gričevje ter prost dostop [mikroskop zaslomba ter regres pomočnik](https://aka.ms/SaRA_OfficeSCA_M365Portal) umestiti urad 365 proplus v porazdeliti računalo activation način.</span><span class="sxs-lookup"><span data-stu-id="89e1b-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="89e1b-108">Če želite več informacij o predpogojih, navodilih za namestitev in smernicah za prilagojene namestitve z orodjem za uvajanje Officea, glejte [uvajanje officea 365 ProPlus z uporabo storitev oddaljenega namizja](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="89e1b-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="89e1b-109">Če želite popraviti napake, povezane z aktiviranjem računalnika v skupni rabi:</span><span class="sxs-lookup"><span data-stu-id="89e1b-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="89e1b-110">Glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="89e1b-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="89e1b-111">Glej [prikrivati urad 365 ProPlus activation stanje](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="89e1b-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="89e1b-112">Če želite namestiti Office 365 ProPlus na RDS iz Microsoft 365 skrbniškega centra, ***ki uporablja privzete nastavitve namestitve***, uporabite naslednje korake:</span><span class="sxs-lookup"><span data-stu-id="89e1b-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="89e1b-113">Preverite, kaj Office 365 načrt imate.</span><span class="sxs-lookup"><span data-stu-id="89e1b-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="89e1b-114">[Naučite se kako](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="89e1b-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="89e1b-115">Če je potrebno, preklopite na drug paket Office 365.</span><span class="sxs-lookup"><span data-stu-id="89e1b-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="89e1b-116">[Naučite se kako](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="89e1b-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="89e1b-117">Če je Office že nameščen v strežniku RDS z uporabo katerega koli drugega programa Office 365, ga odstranite.</span><span class="sxs-lookup"><span data-stu-id="89e1b-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="89e1b-118">Na primer, z tekoč v **pregled svet** > **uninstall a disciplinski nadzornik v Oxfordu ali Cambridgeu**.</span><span class="sxs-lookup"><span data-stu-id="89e1b-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="89e1b-119">Odstranite z [Microsoftovim pomočnikom za podporo in obnovitev](https://aka.ms/SARA-OfficeUninstall-Alchemy) , če izvajate težave.</span><span class="sxs-lookup"><span data-stu-id="89e1b-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="89e1b-120">V strežniku RDS se vpišite v skrbniško središče Microsoft 365 s skrbniškim računom in [namestite Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="89e1b-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="89e1b-121">Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove aplikacije.</span><span class="sxs-lookup"><span data-stu-id="89e1b-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="89e1b-122">V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="89e1b-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="89e1b-123">Z desno miškino tipko kliknite gumb Windows v spodnjem levem kotu zaslona in izberite **Zaženi**.</span><span class="sxs-lookup"><span data-stu-id="89e1b-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="89e1b-124">V polje Odpri vnesite **regedit**in nato izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="89e1b-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="89e1b-125">Izberite **da** , ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.</span><span class="sxs-lookup"><span data-stu-id="89e1b-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="89e1b-126">V urejevalniku registra dodajte vrednost niza» **Sharedcomputerlicensing** «z nastavitvijo 1 pod HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="89e1b-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="89e1b-127">V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="89e1b-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

