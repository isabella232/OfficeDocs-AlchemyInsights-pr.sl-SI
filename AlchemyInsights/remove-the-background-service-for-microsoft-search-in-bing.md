---
title: Odstranjevanje storitve za ozadje za Microsoft Search v storitvi Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816338"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="91e84-102">Odstranjevanje storitve za ozadje za Microsoft Search v storitvi Bing</span><span class="sxs-lookup"><span data-stu-id="91e84-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="91e84-103">Če želite odstraniti storitev za ozadje za Microsoft Search v storitvi Bing, lahko poskusite s temi sredstvi:</span><span class="sxs-lookup"><span data-stu-id="91e84-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="91e84-104">Če želite obnoviti prvotne nastavitve mehanizma za iskanje, naredite nekaj od tega:</span><span class="sxs-lookup"><span data-stu-id="91e84-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="91e84-105">v.</span><span class="sxs-lookup"><span data-stu-id="91e84-105">a.</span></span> <span data-ttu-id="91e84-106">Preklapljanje med **uporabo storitve Bing kot privzetega [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) mehanizma za iskanje izklopite**.</span><span class="sxs-lookup"><span data-stu-id="91e84-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="91e84-107">b.</span><span class="sxs-lookup"><span data-stu-id="91e84-107">b.</span></span> <span data-ttu-id="91e84-108">[Pojdite v skrbniško središče za Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) in počistite nastavitev, ki vpliva na vse uporabnike v vaši organizaciji.</span><span class="sxs-lookup"><span data-stu-id="91e84-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="91e84-109">Če želite odstraniti storitev za ozadje iz posamezne naprave, naredite ta opravila:</span><span class="sxs-lookup"><span data-stu-id="91e84-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="91e84-110">v.</span><span class="sxs-lookup"><span data-stu-id="91e84-110">a.</span></span> <span data-ttu-id="91e84-111">Izberite **Nadzorna plošča > programi > programi in funkcijami**.</span><span class="sxs-lookup"><span data-stu-id="91e84-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="91e84-112">b.</span><span class="sxs-lookup"><span data-stu-id="91e84-112">b.</span></span> <span data-ttu-id="91e84-113">Z desno tipko miške kliknite **Microsoft Search v storitvi Bing** pod seznamom nameščenih programov, nato pa kliknite **Odstrani**.</span><span class="sxs-lookup"><span data-stu-id="91e84-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="91e84-114">Če želite odstraniti storitev za ozadje iz več naprav v organizaciji, se prijavite kot skrbnik in zaženite ta ukaz v skriptu:</span><span class="sxs-lookup"><span data-stu-id="91e84-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
