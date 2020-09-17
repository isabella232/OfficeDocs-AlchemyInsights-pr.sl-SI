---
title: Uporaba orodja za uvajanje sistema Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794927"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="a9ea0-102">Uporaba orodja za uvajanje sistema Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a9ea0-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a9ea0-103">Z orodjem za uvedbo sistema Office (ODT) lahko uvedete Office 365 različice Officea.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="a9ea0-104">Orodje za uvajanje sistema Office (setup.exe) se izvaja v ukazni vrstici in uporablja datoteko konfiguracijske datoteke XML, da določi, katere nastavitve uporabiti pri uvajanju Officea.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="a9ea0-105">Prenesite najnovejšo različico orodja za uvedbo sistema Office iz [Microsoftovega središča za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a9ea0-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="a9ea0-106">Z [orodjem za prilagajanje sistema Office (okt)](https://config.office.com) izberite nastavitve uvajanja in ustvarite datoteko XML za konfiguracijo.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="a9ea0-107">Izvozite konfiguracijsko datoteko in jo postavite na lokalno mesto v isti mapi, kjer setup.exe prebiva.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="a9ea0-108">**Opomba:** Težave z namestitvijo Officea se običajno pojavijo zaradi napačno konfiguriranih ali malformatted konfiguracijskih datotek.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="a9ea0-109">Če se želite izogniti takim težavam, vam priporočamo, da ustvarite konfiguracijsko datoteko z orodjem za prilagajanje sistema Office.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="a9ea0-110">Obstoječe konfiguracijske datoteke lahko uvozite tudi v Officeovo orodje za prilagajanje.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="a9ea0-111">V ukazu» visok ukazni poziv «preklopite na mesto, kjer setup.exe prebiva, in zaženite orodje za uvajanje sistema Office v načinu za prenos in določite konfiguracijsko datoteko, ki ste jo pravkar shranili.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="a9ea0-112">V tem primeru je konfiguracijska datoteka imenovana Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="a9ea0-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="a9ea0-113">4. zaženite orodje za uvedbo sistema Office v načinu Konfiguriraj in določite konfiguracijsko datoteko.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="a9ea0-114">**Opomba:** Ta korak morate zagnati iz odjemalskega računalnika, v katerem želite namestiti Office, in morate imeti dovoljenja lokalnih skrbnikov v tem računalniku.</span><span class="sxs-lookup"><span data-stu-id="a9ea0-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="a9ea0-115">Če želite izvedeti več o uporabi orodja za uvajanje sistema Office za aplikacije Microsoft 365 apps za uvajanje, glejte [pregled orodja za uvedbo sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="a9ea0-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="a9ea0-116">Če želite več informacij o uporabi orodja za prilagajanje sistema Office, glejte [pregled orodja za prilagajanje sistema Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="a9ea0-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
