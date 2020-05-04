---
title: Uporaba Officeovega orodja za uvajanje
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010886"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="759a6-102">Uporaba orodja za uvajanje Officea (ODT)</span><span class="sxs-lookup"><span data-stu-id="759a6-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="759a6-103">Officeovo orodje za razmestitev (ODT) uporabite za uvajanje Officeovih različic 365.</span><span class="sxs-lookup"><span data-stu-id="759a6-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="759a6-104">Officeovo orodje za razmestitev (setup. exe) se zažene iz ukazne vrstice in uporablja konfiguracijsko datoteko XML, da določi, katere nastavitve naj se uporabijo pri uvajanju Officea.</span><span class="sxs-lookup"><span data-stu-id="759a6-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="759a6-105">Prenesite najnovejšo različico orodja za uvajanje Officea iz [Microsoftovega centra za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="759a6-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="759a6-106">Z [orodjem za prilagajanje Office (Oct)](https://config.office.com) izberite nastavitve uvajanja in ustvarite KONFIGURACIJSKO datoteko XML.</span><span class="sxs-lookup"><span data-stu-id="759a6-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="759a6-107">Izvozite konfiguracijsko datoteko in jo postavite lokalno v isto mapo, kjer se nahaja setup. exe.</span><span class="sxs-lookup"><span data-stu-id="759a6-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="759a6-108">**Opomba:** Težave z namestitvijo Officea se pogosto pojavijo zaradi napačnih konfiguriranih ali nepravilno oblikovanih konfiguracijskih datotek.</span><span class="sxs-lookup"><span data-stu-id="759a6-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="759a6-109">Da bi se izognili takim težavam, priporočamo, da za ustvarjanje konfiguracijske datoteke uporabite orodje Office customization Tool.</span><span class="sxs-lookup"><span data-stu-id="759a6-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="759a6-110">Obstoječe konfiguracijske datoteke lahko uvozite tudi v orodje za prilagajanje Officea.</span><span class="sxs-lookup"><span data-stu-id="759a6-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="759a6-111">Iz povišanega ukaznega poziva preklopite na mesto, kjer se nahaja setup. exe, in zaženite orodje za uvajanje Officea v načinu prenosa in določite konfiguracijsko datoteko, ki ste jo pravkar shranili.</span><span class="sxs-lookup"><span data-stu-id="759a6-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="759a6-112">V tem primeru je konfiguracijska datoteka imenovana konfiguracija. XML:</span><span class="sxs-lookup"><span data-stu-id="759a6-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="759a6-113">Zaženite orodje za uvajanje Officea v načinu konfiguriranja in določite konfiguracijsko datoteko.</span><span class="sxs-lookup"><span data-stu-id="759a6-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="759a6-114">**Opomba:** Ta korak morate zagnati v odjemalskem računalniku, v katerem želite namestiti Office, in v tem računalniku morate imeti dovoljenja lokalnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="759a6-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="759a6-115">Če želite izvedeti več o uporabi Officeovega orodja za uvajanje za Microsoft 365 aplikacije za scenarije uvajanja za podjetja, glejte [pregled orodja za uvajanje Officea](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="759a6-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="759a6-116">Če želite več podrobnosti o uporabi orodja za prilagajanje Office, glejte [pregled orodja za prilagajanje Officea](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="759a6-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
