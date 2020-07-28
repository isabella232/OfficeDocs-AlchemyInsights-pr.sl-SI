---
title: Nadzor samodejnih posodobitev za Officeove programe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439925"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="11ccd-102">Nadzor samodejnih posodobitev za Officeove programe</span><span class="sxs-lookup"><span data-stu-id="11ccd-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="11ccd-103">Posodobitve za Officeove aplikacije se privzeto samodejno prenesejo in uporabijo v ozadju brez posredovanja uporabnika.</span><span class="sxs-lookup"><span data-stu-id="11ccd-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="11ccd-104">Vendar pa lahko skrbniki nadzirajo, kako se posodobitve uporabljajo z nastavitvami storitve Office Update.</span><span class="sxs-lookup"><span data-stu-id="11ccd-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="11ccd-105">Nastavitve posodobitve skrbnikom omogočajo, da omogočijo ali onemogočijo samodejne posodobitve, **prikažejo ali skrijejo gumb Posodobi zdaj** v Officeu, nastavijo roke za posodobitev in še več.</span><span class="sxs-lookup"><span data-stu-id="11ccd-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="11ccd-106">Za podrobnejše informacije glej:</span><span class="sxs-lookup"><span data-stu-id="11ccd-106">For detailed information, see:</span></span>

- [<span data-ttu-id="11ccd-107">Konfiguracija nastavitev posodobitve za Office</span><span class="sxs-lookup"><span data-stu-id="11ccd-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="11ccd-108">Samodejno posodabljanje za Office ni omogočeno</span><span class="sxs-lookup"><span data-stu-id="11ccd-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="11ccd-109">Določanje načina posodablja glede na to, kako se Office posodobi po namestitvi</span><span class="sxs-lookup"><span data-stu-id="11ccd-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="11ccd-110">Če želite pregledati obstoječe nastavitve posodobitev, ki veljajo za odjemalski računalnik, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="11ccd-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="11ccd-111">plan registracija urednik z tekoč v **začetek prost**  >  **dostop**  >  **zopet zmrzniti**.</span><span class="sxs-lookup"><span data-stu-id="11ccd-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="11ccd-112">Preklopite na to mesto in preglejte nastavitve storitve Office Update:</span><span class="sxs-lookup"><span data-stu-id="11ccd-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="11ccd-113">A.</span><span class="sxs-lookup"><span data-stu-id="11ccd-113">a.</span></span> <span data-ttu-id="11ccd-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="11ccd-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="11ccd-115">B.</span><span class="sxs-lookup"><span data-stu-id="11ccd-115">b.</span></span> <span data-ttu-id="11ccd-116">Kliknite »Run\Configuration«</span><span class="sxs-lookup"><span data-stu-id="11ccd-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="11ccd-117">\*\* Opomba\*\*  Če je ključ OfficeMgmtCOM nastavljen, se lahko v officeovih posodobitvah za račun officea prikaže sporočilo **»Posodobitve**upravlja skrbnik  >  **Account**  >  **sistema«.**</span><span class="sxs-lookup"><span data-stu-id="11ccd-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="11ccd-118">Če želite več informacij, [glejte Upravljanje posodobitev za programe Microsoft 365 z Microsoft Endpoint Configuration Managerjem](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="11ccd-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  