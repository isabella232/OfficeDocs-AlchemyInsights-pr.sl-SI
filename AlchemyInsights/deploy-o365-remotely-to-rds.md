---
title: Uvajanje programov Microsoft 365 za podjetja za uporabo v skupni rabi v programu RDS, Terminal Server ali VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200689"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="2f8ce-102">Uvajanje programov Microsoft 365 za podjetja za uporabo v skupni rabi v programu RDS, Terminal Server ali VDI</span><span class="sxs-lookup"><span data-stu-id="2f8ce-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="2f8ce-103">Če želite uvesti aplikacije Microsoft 365 za podjetja z oddaljenimi namiznimi storitvami (RDS), ki so bile prej imenovane terminalske storitve:</span><span class="sxs-lookup"><span data-stu-id="2f8ce-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="2f8ce-104">Imeti morate paket Microsoft 365 za podjetja ali paket Office 365, ki vključuje aplikacije Microsoft 365 za podjetja, kot so Office 365 Enterprise E3 ali Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="2f8ce-105">Microsoft 365 apps za podjetja in Microsoft 365 Business standard paketi ne vključujejo programov Microsoft 365 za podjetja.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="2f8ce-106">Omogočiti morate [aktiviranje računalnika v skupni rabi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="2f8ce-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="2f8ce-107">Prav tako lahko prenesete in zaženete [Microsoftov pomočnik za podporo in obnovitev](https://aka.ms/SaRA_OfficeSCA_M365Portal) , da namestite Microsoft 365 apps za podjetja v načinu za aktiviranje računalnika v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="2f8ce-108">Če želite več informacij o predpogojih, navodilih za nastavitev in usmerjanju po prilagojenih napravah z orodjem za uvedbo sistema Office, glejte [uvajanje programov Microsoft 365 za podjetja z oddaljenimi namiznimi storitvami](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="2f8ce-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="2f8ce-109">Odpravljanje napak, povezanih s aktiviranjem računalnika v skupni rabi:</span><span class="sxs-lookup"><span data-stu-id="2f8ce-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="2f8ce-110">Glejte [Odpravljanje težav z aktiviranjem računalnika v skupni rabi za Microsoft 365 apps za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="2f8ce-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="2f8ce-111">Glejte [Ponastavite stanje aktiviranja naročnine Aplikacije ogrodja Microsoft 365 za podjetja](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="2f8ce-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="2f8ce-112">Če želite namestiti aplikacije Microsoft 365 za podjetja v programu RDS v skrbniškem središču za Microsoft 365, ***ki uporablja privzete nastavitve namestitve***, uporabite te korake:</span><span class="sxs-lookup"><span data-stu-id="2f8ce-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="2f8ce-113">Preverite, katero naročnino imate.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-113">Check what subscription you have.</span></span> <span data-ttu-id="2f8ce-114">[Preberite več o](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)tem.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="2f8ce-115">Po potrebi preklopite na drugo naročnino.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="2f8ce-116">[Preberite več o](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)tem.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="2f8ce-117">Če je Office že nameščen v strežniku RDS s katero koli drugo Microsoftovo naročnino, ga odstranite.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="2f8ce-118">Na primer, če želite   >  **odstraniti program** na nadzorni plošči.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="2f8ce-119">Odstranite s pomočjo [Microsoftovega pomočnika za podporo in obnovitev,](https://aka.ms/SARA-OfficeUninstall-Alchemy) če se izvaja težave.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="2f8ce-120">V strežniku RDS se vpišite v skrbniško središče za Microsoft 365 s skrbniškim računom in [namestite Microsoft 365 aplikacije za podjetja](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="2f8ce-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="2f8ce-121">Ko je Office nameščen, se ***ne odpirajte ali vpišite v*** Officeove programe.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="2f8ce-122">V strežniku RDS omogočite aktiviranje računalnika v skupni rabi tako, da uredite register tako, da upoštevate te korake:</span><span class="sxs-lookup"><span data-stu-id="2f8ce-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="2f8ce-123">Z desno tipko miške kliknite gumb sistema Windows v spodnjem levem kotu zaslona in izberite **Zaženi**.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="2f8ce-124">V polje Odpri vnesite **regedit** in nato izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="2f8ce-125">Izberite **da** , ko ste pozvani, da omogočite urejevalnik registra, da spremenite vašo napravo.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="2f8ce-126">V urejevalniku registra dodajte vrednost niza **SharedComputerLicensing** z nastavitvami 1 v razdelku HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="2f8ce-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="2f8ce-127">V strežniku RDS se ***vpišite kot končni uporabnik*** in [Preverite, ali je aktiviranje računalnika v skupni rabi omogočeno za programe Microsoft 365 za podjetja](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="2f8ce-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
