---
title: 902 (sinhronizacijske napake zaradi podvojenih predmetov)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507431"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="1073c-102">Sinhronizacijske napake zaradi podvojenih predmetov</span><span class="sxs-lookup"><span data-stu-id="1073c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="1073c-103">Eno od teh sporočil o napaki lahko prejmete, ko sinhronizacija imenika konča v Office 365:</span><span class="sxs-lookup"><span data-stu-id="1073c-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="1073c-104">Ni mogoče posodobiti ta predmet v Microsoft Online Services, ker teh atributov, ki so povezani s tem predmetom so vrednosti, ki lahko že povezano z drugim predmetom, v vaš tukajšnji naslovnik.</span><span class="sxs-lookup"><span data-stu-id="1073c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="1073c-105">Sinhroniziranega predmeta z isto zastopstvo ogovor že obstaja v imeniku Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="1073c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="1073c-106">Mogoče posodobiti ta predmet, ker teh atributov, ki so povezani s tem predmetom so vrednosti, ki lahko že povezano z drugim predmetom, v vaš tukajšnji naslovnik storitve: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1073c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="1073c-107">Prepoznajte in odpravite težavo, prenesite in zaženite [Orodje za sanacijo IdFix DirSync napake](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="1073c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="1073c-108">Če želite več informacij, glejte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="1073c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
