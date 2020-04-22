---
title: Omejevanje dostopa v SharePointu ali storitvi OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715900"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="2d8ca-102">Omejevanje dostopa v SharePointu ali storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="2d8ca-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="2d8ca-103">V SharePointu in storitvi OneDrive omejite dostop do elementov, kot so datoteke, mape in seznami, tako da omogočite dostop samo skupinam ali posameznikom, ki jih želite imeti dostop.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="2d8ca-104">Dovoljenja v SharePointu so privzeto podedovana od višje v hierarhiji.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="2d8ca-105">Torej datoteka dedi dovoljenja iz mape, ki dedi dovoljenja iz knjižnice, ki dedi svoja dovoljenja iz mesta.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="2d8ca-106">Lahko delite na višji ravni (na primer z delitvijo celotno mesto) in nato prekinil dedovanje, če ne želite deliti vse elemente na mestu.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="2d8ca-107">Vendar pa tega ne priporočamo, ker omogoča ohranitev dovoljenj bolj zapletena in nejasna v prihodnosti.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="2d8ca-108">Tukaj je, kaj lahko storite namesto tega:</span><span class="sxs-lookup"><span data-stu-id="2d8ca-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="2d8ca-109">Če želite na primer deliti vso vsebino mape, razen ene datoteke v njej, premaknite to datoteko na novo mesto, ki ni v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="2d8ca-110">Če imate v mapi dve podmapi in želite deliti eno podmapo s skupinami A in B in dovoliti samo skupini A dostop do druge podmape, delite nadrejeno mapo s skupino A in dodajte skupino B v prvo podmapo.</span><span class="sxs-lookup"><span data-stu-id="2d8ca-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="2d8ca-111">Ustavitev skupne rabe datoteke ali mape</span><span class="sxs-lookup"><span data-stu-id="2d8ca-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

