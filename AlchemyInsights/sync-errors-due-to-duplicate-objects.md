---
title: 902 (napake sinhronizacije zaradi podvojenih predmetov)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737357"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="1000f-102">Napake sinhronizacije zaradi podvojenih predmetov</span><span class="sxs-lookup"><span data-stu-id="1000f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="1000f-103">Ko se sinhronizacija imenika konča v programu Microsoft 365, se lahko prikaže eno od teh sporočil o napaki:</span><span class="sxs-lookup"><span data-stu-id="1000f-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="1000f-104">Tega predmeta ni mogoče posodobiti v storitvi Microsoft Online Services, ker so v teh atributih, povezanih s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v lokalnem imeniku.</span><span class="sxs-lookup"><span data-stu-id="1000f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="1000f-105">Sinhroniziran predmet z istim naslovom strežnika proxy že obstaja v vašem imeniku storitve Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="1000f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="1000f-106">Tega predmeta ni mogoče posodobiti, ker so v teh atributih, povezanih s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v lokalnih imeniških storitvah: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1000f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="1000f-107">Če želite prepoznati in odpraviti težavo, prenesite in zaženite [orodje za sanacijo napak v IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="1000f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="1000f-108">Če želite več informacij, glejte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="1000f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
