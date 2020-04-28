---
title: Podvojitev zapisov naprav v portalu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790173"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="3ab07-102">Podvojitev zapisov naprav v portalu</span><span class="sxs-lookup"><span data-stu-id="3ab07-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="3ab07-103">V portalu boste morda videli 2 zapisa za napravo, če naprava spletnemu mestu upravitelja konfiguracije trenutno ne poroča stanja soupravljanja.</span><span class="sxs-lookup"><span data-stu-id="3ab07-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="3ab07-104">Če želite preveriti stanje soupravljanja naprave, si oglejte stolpec **Soupravljano** za napravo v konzoli upravitelja konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="3ab07-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="3ab07-105">Če stolpec ni viden, ga lahko dodate tako, da z desno tipko miške kliknite glave stolpcev in ga izberete na seznamu.</span><span class="sxs-lookup"><span data-stu-id="3ab07-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="3ab07-106">Vrednost soupravljanja mora biti **Da**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="3ab07-107">Če je vrednost **Ne**, odprite aplikacijo odjemalca upravitelja konfiguracije v odjemalski napravi in preverite vrednost lastnosti **Soupravljanje** na zavihku »Splošno«.</span><span class="sxs-lookup"><span data-stu-id="3ab07-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="3ab07-108">Če je vrednost **Omogočeno**, kaže to na težave pri komunikaciji odjemalca s točko upravljanja.</span><span class="sxs-lookup"><span data-stu-id="3ab07-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="3ab07-109">Če želite poiskati morebitne težave s povezljivostjo, preglejte dnevnik **CcmMessaging.log** v napravi.</span><span class="sxs-lookup"><span data-stu-id="3ab07-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="3ab07-110">Če je vrednost **Onemogočeno**, naprava pa je včlanjena v Intune, preverite, ali je naprava prejela pravilnik o soupravljanju. To naredite tako, da v napravi pregledate dnevnik **CoManagementHandler.log**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
