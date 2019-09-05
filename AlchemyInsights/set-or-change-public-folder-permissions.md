---
title: Nastavljanje ali spreminjanje dovoljenj za javno mapo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734685"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="56fc5-102">Dovoljenja in javne mape</span><span class="sxs-lookup"><span data-stu-id="56fc5-102">Permissions and Public Folders</span></span>

<span data-ttu-id="56fc5-103">Dovoljenja v javnih mapah lahko spremenite z Outlookom, skrbniškim centrom Exchange (EAC) ali lupino PowerShell:</span><span class="sxs-lookup"><span data-stu-id="56fc5-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="56fc5-104">Za Outlookova navodila [Kliknite tukaj](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="56fc5-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="56fc5-105">Za EAC glejte [Ta članek](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) za navodila.</span><span class="sxs-lookup"><span data-stu-id="56fc5-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="56fc5-106">Zakaj PowerShell, nanašati se na [to člen](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) zakaj navodila naprej using povečati-PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="56fc5-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="56fc5-107">Če potrebujete navodila za vzpostavljanje povezave z Exchangeevim PowerShell, kliknite [tukaj](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="56fc5-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="56fc5-108">Če **zunanji uporabniki ne morejo pošiljati e-poštnih sporočil v javno mapo z omogočeno pošto**, je morda razlog za to, da javna mapa manjka dovoljenja, potrebna za zunanjo dostavo e-pošte.</span><span class="sxs-lookup"><span data-stu-id="56fc5-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="56fc5-109">To lahko odpravite s pomočjo Outlookovih navodil [tukaj](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)ali navodilom PowerShell [tukaj](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="56fc5-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

