---
title: Lastnik ne more ustvariti podmape z Outlookom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836151"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="54c5a-102">Lastnik ne more ustvariti podmape z Outlookom</span><span class="sxs-lookup"><span data-stu-id="54c5a-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="54c5a-103">**Trenutno obstaja težava z ustvarjanjem podmap v Outlooku z lastniki javnih map. Ta težava bo kmalu odpravljena.**</span><span class="sxs-lookup"><span data-stu-id="54c5a-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="54c5a-104">Medtem pa uporabite eno od teh rešitev:</span><span class="sxs-lookup"><span data-stu-id="54c5a-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="54c5a-105">Uporabite Outlook za MAC, da ustvarite podmapo, saj težava vpliva le na Outlook za namizno različico okna (vse različice)</span><span class="sxs-lookup"><span data-stu-id="54c5a-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="54c5a-106">Naj skrbnik ustvari podmapo z lupino EXO ali EAC</span><span class="sxs-lookup"><span data-stu-id="54c5a-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="54c5a-107">Spreminjanje mape DefaultPublicFolderMailbox/EffectivePublicFolderMailbox za uporabnika v drug nabiralnik in ne v nabiralnik vsebine za mapo, ki povzroča težavo</span><span class="sxs-lookup"><span data-stu-id="54c5a-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="54c5a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="54c5a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="54c5a-109">Počakajte eno uro, znova zaženite Outlookovega odjemalca</span><span class="sxs-lookup"><span data-stu-id="54c5a-109">Wait for an hour, restart outlook client</span></span>