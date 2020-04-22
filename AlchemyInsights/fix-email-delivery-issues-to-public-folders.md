---
title: Odpravljanje težav z dostavo e-pošte v javne mape z omogočeno pošto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716368"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="3ae3d-102">Odpravljanje težav z dostavo e-pošte v javne mape z omogočeno pošto</span><span class="sxs-lookup"><span data-stu-id="3ae3d-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="3ae3d-103">Če zunanji pošiljatelji ne morejo pošiljati sporočil v javne mape z omogočenimi poštnimi sporočili, pošiljatelji pa prejmejo napako: **ni bilo mogoče najti (550 5.4.1)**, preveriti, ali je domena e-pošte za javno mapo konfigurirana kot notranja domena releja namesto avtoritativne domene:</span><span class="sxs-lookup"><span data-stu-id="3ae3d-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="3ae3d-104">Odprite [skrbniško središče za Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="3ae3d-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="3ae3d-105">Pojdite na e- **poštni tok** \> **sprejete domene**, izberite sprejeto domeno in nato kliknite **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="3ae3d-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="3ae3d-106">Na strani z lastnostmi, ki se odpre, če je vrsta domene nastavljena na **avtoritativno**, spremenite vrednost v **notranji rele** in nato kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="3ae3d-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="3ae3d-107">Če zunanji pošiljatelji prejmejo napako, ki je nimate **dovoljenja (550 5.7.13)**, zaženite ta ukaz v [PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , da si ogledate dovoljenja za anonimne uporabnike v javni mapi:</span><span class="sxs-lookup"><span data-stu-id="3ae3d-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="3ae3d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="3ae3d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="3ae3d-109">Če želite zunanjim uporabnikom omogočiti pošiljanje e-pošte v to javno mapo, dodajte pravico do dostopa CreateItems uporabniku anonimno.</span><span class="sxs-lookup"><span data-stu-id="3ae3d-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="3ae3d-110">Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="3ae3d-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
