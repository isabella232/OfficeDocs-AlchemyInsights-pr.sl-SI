---
title: Popraviti vprašanja dostave e-pošte za poštne javne mape
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387721"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="eaf42-102">Popraviti vprašanja dostave e-pošte za poštne javne mape</span><span class="sxs-lookup"><span data-stu-id="eaf42-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="eaf42-103">Če zunanjih pošiljateljev ne more pošiljati sporočil pošto javnih map, in oddajnik napaki: **ni bilo mogoče najti (550 5.4.1)**, preverite e-poštni domeni za javne mape je konfiguriran kot notranjo domeno za posredovanje namesto na avtoritativno domeno:</span><span class="sxs-lookup"><span data-stu-id="eaf42-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="eaf42-104">Odprite [izmenjavo admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="eaf42-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="eaf42-105">Pojdi na **tok pošte** \> **sprejeto domene**, izberite sprejeto domeno, in nato kliknite **Urejanje**.</span><span class="sxs-lookup"><span data-stu-id="eaf42-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="eaf42-106">V lastnosti strani odpre, če domene tipa **Authoritative**, spremenite vrednost za **notranje posredovanje** in kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="eaf42-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="eaf42-107">Če zunanjih pošiljateljev prikaže napaka, **nimate dovoljenja (550 5.7.13)**, zaženite ta ukaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , da vidite, katera dovoljenja za anonimne uporabnike v javni mapi:</span><span class="sxs-lookup"><span data-stu-id="eaf42-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="eaf42-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="eaf42-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="eaf42-109">Zunanjim uporabnikom pošiljati email v tej javni mapi, dodajte CreateItems dostop pravico do uporabnika Anonymous.</span><span class="sxs-lookup"><span data-stu-id="eaf42-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="eaf42-110">Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="eaf42-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
