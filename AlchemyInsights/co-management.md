---
title: Soupravljanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910446"
---
# <a name="co-management"></a><span data-ttu-id="1dc72-102">Soupravljanje</span><span class="sxs-lookup"><span data-stu-id="1dc72-102">Co-management</span></span>

<span data-ttu-id="1dc72-103">**Predpogoj za selitev iz config Manager Hybrid za InTune**</span><span class="sxs-lookup"><span data-stu-id="1dc72-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="1dc72-104">Preglejte [Ta članek](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span><span class="sxs-lookup"><span data-stu-id="1dc72-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="1dc72-105">[Uporabnikom dodajte licenco InTune](https://docs.microsoft.com/intune/licenses-assign).</span><span class="sxs-lookup"><span data-stu-id="1dc72-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="1dc72-106">Pri konfiguriranju soupravljanja uporabite [brskalnik Edge](https://www.microsoft.com/windows/microsoft-edge) .</span><span class="sxs-lookup"><span data-stu-id="1dc72-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="1dc72-107">**Kako namestiti odjemalca config Manager na InTune-upravljane naprave**</span><span class="sxs-lookup"><span data-stu-id="1dc72-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="1dc72-108">Glejte [InTune naprave s sistemom Windows, ki jih upravlja MDM](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span><span class="sxs-lookup"><span data-stu-id="1dc72-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="1dc72-109">**Kaj pa, če želim spremeniti MDM organ?**</span><span class="sxs-lookup"><span data-stu-id="1dc72-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="1dc72-110">MDM organ se lahko spremeni, ne da bi odprli podporni primer.</span><span class="sxs-lookup"><span data-stu-id="1dc72-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="1dc72-111">Prosimo, preglejte naslednjo dokumentacijo za pomoč pri spreminjanju svojega organa MDM:</span><span class="sxs-lookup"><span data-stu-id="1dc72-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="1dc72-112">Sprememba MDM pooblastilo s config šef v InTune standalone</span><span class="sxs-lookup"><span data-stu-id="1dc72-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="1dc72-113">Sprememba MDM pooblastilo s InTune standalone v config šef</span><span class="sxs-lookup"><span data-stu-id="1dc72-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)