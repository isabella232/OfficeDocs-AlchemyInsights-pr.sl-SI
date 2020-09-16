---
title: Omejevanje dostopa v SharePointu ali OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720698"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="09afc-102">Omejevanje dostopa v SharePointu ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="09afc-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="09afc-103">V SharePointu in OneDrive omejite dostop do elementov, kot so datoteke, mape in seznami, tako da podelite dostop le skupinam ali posameznikom, za katere želite imeti dostop.</span><span class="sxs-lookup"><span data-stu-id="09afc-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="09afc-104">Dovoljenja v SharePointu so privzeto podedovana od višjega v hierarhiji.</span><span class="sxs-lookup"><span data-stu-id="09afc-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="09afc-105">Tako datoteka podeduje dovoljenja iz mape, ki deduje dovoljenja iz knjižnice, ki deduje dovoljenja na mestu.</span><span class="sxs-lookup"><span data-stu-id="09afc-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="09afc-106">Daste lahko v skupno rabo na višji ravni (na primer s skupno rabo celotnega mesta), nato pa razdelite dedovanje, če ne želite dati vseh elementov na mestu.</span><span class="sxs-lookup"><span data-stu-id="09afc-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="09afc-107">Vendar pa tega ne priporočamo, ker je v prihodnosti treba ohraniti dovoljenja, ki so bolj zapletena in zavajajoča.</span><span class="sxs-lookup"><span data-stu-id="09afc-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="09afc-108">Naredite lahko to:</span><span class="sxs-lookup"><span data-stu-id="09afc-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="09afc-109">Če na primer želite dati v skupno rabo vso vsebino mape, razen ene datoteke v njej, premaknite to datoteko na novo mesto, ki ni v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="09afc-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="09afc-110">Če imate v mapi dve podmapi in želite dati v skupno rabo eno podmapo s skupinami A in B in omogočiti le dostop do druge podmape, skupna raba nadrejene mape s skupino A in dodajanje skupine B v prvo podmapo.</span><span class="sxs-lookup"><span data-stu-id="09afc-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="09afc-111">Ustavitev skupne rabe datoteke ali mape </span><span class="sxs-lookup"><span data-stu-id="09afc-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

