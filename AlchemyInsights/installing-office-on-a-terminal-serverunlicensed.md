---
title: Namestitev Officea v terminalski strežnik – brez licence
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663133"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8abe6-102">Namestitev Officea v terminalski strežnik</span><span class="sxs-lookup"><span data-stu-id="8abe6-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8abe6-103">Za uvajanje programov Microsoft 365 za podjetja v sistemu Windows Server z oddaljenimi namiznimi storitvami (RDS), prej imenovanimi terminalskih storitev:</span><span class="sxs-lookup"><span data-stu-id="8abe6-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8abe6-104">Imeti morate naročnino na Microsoftovo 365, ki vključuje aplikacije Microsoft 365 za podjetja, kot so Office 365 Enterprise E3 ali Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8abe6-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8abe6-105">Microsoft 365 apps za podjetja in Microsoft 365 apps za pakete za podjetja Premium ne vključujejo programov Microsoft 365 za podjetja.</span><span class="sxs-lookup"><span data-stu-id="8abe6-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="8abe6-106">Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8abe6-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="8abe6-107">Če želite namestiti aplikacije Microsoft 365 za podjetja v programu RDS v skrbniškem središču za Microsoft 365, ***ki uporablja privzete nastavitve namestitve***, uporabite te korake.</span><span class="sxs-lookup"><span data-stu-id="8abe6-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8abe6-108">Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetja v načinu za aktiviranje računalnika v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="8abe6-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8abe6-109">Preverite, katero naročnino na Microsoftovo 365 imate.</span><span class="sxs-lookup"><span data-stu-id="8abe6-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="8abe6-110">Preberite, kako</span><span class="sxs-lookup"><span data-stu-id="8abe6-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8abe6-111">Po potrebi preklopite na drugo naročnino na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8abe6-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="8abe6-112">Preberite, kako</span><span class="sxs-lookup"><span data-stu-id="8abe6-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="8abe6-113">Če je Office že nameščen v strežniku RDS s katero koli drugo naročnino na Microsoft 365, ga odstranite.</span><span class="sxs-lookup"><span data-stu-id="8abe6-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="8abe6-114">Na primer, če želite odstraniti program na nadzorni plošči \> .</span><span class="sxs-lookup"><span data-stu-id="8abe6-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8abe6-115">Odstranite s pomočjo [Microsoftovega pomočnika za podporo in obnovitev,](https://aka.ms/SARA-OfficeUninstall-Alchemy) če se izvaja težave.</span><span class="sxs-lookup"><span data-stu-id="8abe6-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8abe6-116">V strežniku RDS se vpišite v skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 aplikacije za podjetja](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8abe6-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8abe6-117">Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove programe.</span><span class="sxs-lookup"><span data-stu-id="8abe6-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8abe6-118">V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da upoštevate te korake:</span><span class="sxs-lookup"><span data-stu-id="8abe6-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8abe6-119">Z desno tipko miške kliknite gumb sistema Windows v spodnjem levem kotu zaslona in izberite Zaženi.</span><span class="sxs-lookup"><span data-stu-id="8abe6-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8abe6-120">V polje Odpri vnesite **regedit**in nato izberite v redu.</span><span class="sxs-lookup"><span data-stu-id="8abe6-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8abe6-121">Izberite da, ko ste pozvani, da omogočite urejevalnik registra, da spremenite vašo napravo.</span><span class="sxs-lookup"><span data-stu-id="8abe6-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8abe6-122">V urejevalniku registra dodajte vrednost niza **SharedComputerLicensing** z nastavitvami 1 v razdelku HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8abe6-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8abe6-123">V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za programe Microsoft 365 za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8abe6-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="8abe6-124">Če želite več informacij o predpogojih, navodilih za nastavitev in usmerjanju po prilagojenih napravah z orodjem za uvedbo sistema Office, si oglejte [uvajanje programov Microsoft 365 za podjetja z oddaljenimi namiznimi storitvami](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8abe6-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="8abe6-125">Če želite odpraviti napake, povezane z aktiviranjem računalnika v skupni rabi, si oglejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8abe6-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  