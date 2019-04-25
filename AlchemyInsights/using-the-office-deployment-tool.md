---
title: Z orodjem za uvajanje urad
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423199"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="ba0d8-102">Z orodjem za uvajanje Officea (ODT)</span><span class="sxs-lookup"><span data-stu-id="ba0d8-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ba0d8-103">Uporabite orodje Office uvajanja (ODT) za uvedbo Office 365 različice Officea.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="ba0d8-104">Orodjem za uvajanje Officea (setup.exe) izvaja iz ukazne vrstice in uses a konfiguracijske datoteke XML odločiti kaj nastavitve uporabiti pri uvajanju urad.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="ba0d8-105">Prenesite najnovejšo različico Office uvajanje orodja iz [Microsoftovega centra za prenose](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ba0d8-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="ba0d8-106">Uporabite [Office Customization Tool (ČDO)](https://config.office.com) izberite nastavitve uvajanja in ustvarjanje konfiguracijske datoteke XML.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="ba0d8-107">Izvozi konfiguracijsko datoteko in jo postavite lokalno na isti mapi, setup.exe, kjer prebiva.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="ba0d8-108">**Opomba:** Urad umestitev, pogosto pride do težav zaradi da narobe ali konfiguracijske datoteke malformatted.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="ba0d8-109">Izogibati se taka vprašanja, vam priporočamo, da uporabite Office Customization Tool ustvarite konfiguracijsko datoteko.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="ba0d8-110">Lahko tudi uvozite obstoječe konfiguracijske datoteke Office Customization Tool.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="ba0d8-111">Iz visok zapoved uren, preklopite na mestu, kjer setup.exe in zagon orodja za uvajanje urad v travnato gričevje način in določite konfiguracijske datoteke, ki jo pravkar shranili.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="ba0d8-112">V tem primeru je zunanja podoba pila imenovan Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="ba0d8-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="ba0d8-113">Zaženite orodje za uvajanje urad v oblikovati način in določite konfiguracijske datoteke.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="ba0d8-114">**Opomba:** Ta korak morate zagnati odjemalskega računalnika, na katerem želite namestiti Office in v računalniku morate imeti lokalne skrbniške pravice.</span><span class="sxs-lookup"><span data-stu-id="ba0d8-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="ba0d8-115">Če želite izvedeti več o uporabi Officea uvajanje orodja za Office 365 ProPlus scenarijev uvajanja, si oglejte [pregled urad uvajanje orodja](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="ba0d8-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="ba0d8-116">Za več podrobnosti o tem, kako uporabiti Office Customization Tool, si oglejte [pregled Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="ba0d8-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

