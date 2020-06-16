---
title: Lastnik ne more ustvariti podmape z Outlookom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749145"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="faa57-102">Lastnik ne more ustvariti podmape z Outlookom</span><span class="sxs-lookup"><span data-stu-id="faa57-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="faa57-103">**V programu Outlook je Trenutna težava z lastniki javnih map, ki ustvarjajo podmape. Vprašanje bo kmalu določeno.**</span><span class="sxs-lookup"><span data-stu-id="faa57-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="faa57-104">Medtem, raba nedoločni zaimek od sledeč workarounds:</span><span class="sxs-lookup"><span data-stu-id="faa57-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="faa57-105">Uporabite Outlook za MAC ustvariti podmapo, kot je vprašanje vpliva samo Outlook za namizne okna (vse različice)</span><span class="sxs-lookup"><span data-stu-id="faa57-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="faa57-106">Ali admin ustvariti podmapo z uporabo EXO Shell ali EAC</span><span class="sxs-lookup"><span data-stu-id="faa57-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="faa57-107">Spremenite DefaultPublicFolderMailbox/Efetivepublicfoldermailbox na uporabnika v drug nabiralnik kot nabiralnik vsebine za mapo, ki povzroča težavo</span><span class="sxs-lookup"><span data-stu-id="faa57-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="faa57-108">*Set-poštni nabiralnik UPORABNIK1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="faa57-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="faa57-109">Počakajte eno uro, znova zaženite Outlookovo stranko</span><span class="sxs-lookup"><span data-stu-id="faa57-109">Wait for an hour, restart outlook client</span></span>