---
title: Javna mapa» Pošlji kot pošto «v programu EKSO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462073"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="7ae77-102">Javna mapa z omogočeno pošto SendAs</span><span class="sxs-lookup"><span data-stu-id="7ae77-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="7ae77-103">Ta primer dodeli dovoljenja» Pošlji kot «za javno mapo z omogočeno pošto NewPF1 za uporabnika Jason.</span><span class="sxs-lookup"><span data-stu-id="7ae77-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="7ae77-104">Add-RecipientPermission-Identity "NewPF1"-upravitelj "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="7ae77-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="7ae77-105">Če želite podrobne informacije o sintaksi in parametrih, glejte [dodeljevanje dovoljenj» Pošlji kot «ali» Pošlji v imenu «za javne mape z omogočeno pošto](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="7ae77-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

