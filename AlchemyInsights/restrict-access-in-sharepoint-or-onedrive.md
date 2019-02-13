---
title: Omejevanje dostopa v SharePoint ali OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905164"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8af70-102">Omejevanje dostopa v SharePoint ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="8af70-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8af70-p101">V SharePoint in OneDrive, omejite dostop do predmetov, kot so datoteke, mape in sezname z odobritvijo dostopa le za skupine ali posamezniki, ki želite imeti dostop. Privzeto dovoljenja v SharePoint dedujejo iz višje v hierarhiji. Tako datoteko podeduje njena dovoljenja v mapi, ki podeduje njeno dovoljenja iz knjižnice, ki je njena dovoljenja podedovana.</span><span class="sxs-lookup"><span data-stu-id="8af70-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="8af70-p102">Delite na višji ravni (kot z delitvijo celotno spletno mesto) in nato prekiniti dedovanje, če ne želite, da delijo vse elemente na spletni strani. Vendar, ne priporočamo to saj omogoča ohranitev dovoljenja bolj kompleksnih in zavajajoče v prihodnosti. Tukaj je, kaj bi vam namesto tega:</span><span class="sxs-lookup"><span data-stu-id="8af70-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="8af70-109">Če na primer želite deliti vsebino mape, razen za eno datoteko, premakniti to datoteko na novo lokacijo, ki ni v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="8af70-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="8af70-110">Če imate dva podmape v mapi, in želite deliti eno podmapo z skupin A in B in dovoljujejo le skupina A drugi podmapo, delež nadrejeno mapo s skupino A in skupine B dodati prvo podmapo.</span><span class="sxs-lookup"><span data-stu-id="8af70-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="8af70-111">Ustavi skupno rabo datoteko ali mapo</span><span class="sxs-lookup"><span data-stu-id="8af70-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

