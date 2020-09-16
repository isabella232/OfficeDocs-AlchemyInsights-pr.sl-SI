---
title: Lastnik ne more ustvariti podmape z Outlookom
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665734"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="eb132-102">Lastnik ne more ustvariti podmape z Outlookom</span><span class="sxs-lookup"><span data-stu-id="eb132-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="eb132-103">**V nadaljevanju je prišlo do težave z lastniki javnih map, ki ustvarijo podmape z Outlookom. Težava bo kmalu popravljena.**</span><span class="sxs-lookup"><span data-stu-id="eb132-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="eb132-104">Medtem uporabite eno od teh rešitev:</span><span class="sxs-lookup"><span data-stu-id="eb132-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="eb132-105">Uporaba Outlooka za MAC za ustvarjanje podmape kot težave vpliva le na Outlook za namizne Windows (vse različice)</span><span class="sxs-lookup"><span data-stu-id="eb132-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="eb132-106">Ali je skrbnik ustvaril podmapo s funkcijo EKSO Shell ali EAC</span><span class="sxs-lookup"><span data-stu-id="eb132-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="eb132-107">Spreminjanje DefaultPublicFolderMailbox/EffectivePublicFolderMailbox uporabnika v drugega nabiralnika, kot je nabiralnik vsebine za mapo, ki povzroča težavo</span><span class="sxs-lookup"><span data-stu-id="eb132-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="eb132-108">*Nastavitev nabiralnika UPORABNIK1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="eb132-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="eb132-109">Počakajte eno uro, znova zaženite Outlook Client</span><span class="sxs-lookup"><span data-stu-id="eb132-109">Wait for an hour, restart outlook client</span></span>