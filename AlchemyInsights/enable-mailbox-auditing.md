---
title: Omogočanje revizije nabiralnika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736269"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="6d46e-102">Omogočanje revizije nabiralnika</span><span class="sxs-lookup"><span data-stu-id="6d46e-102">Enable mailbox auditing</span></span>

<span data-ttu-id="6d46e-103">Če želite omogočiti nadzor nabiralnika za enega samega uporabnika ali celotno organizacijo, mora ta ukaz» cmdlet «zagnati iz oddaljene lupine:</span><span class="sxs-lookup"><span data-stu-id="6d46e-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="6d46e-104">**En uporabnik**</span><span class="sxs-lookup"><span data-stu-id="6d46e-104">**Single User**</span></span>
  
<span data-ttu-id="6d46e-105">Set-Mailbox-identiteta "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="6d46e-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="6d46e-106">**Organizacija**</span><span class="sxs-lookup"><span data-stu-id="6d46e-106">**Organization**</span></span>
  
<span data-ttu-id="6d46e-107">Get-nabiralnik-ResultSize neomejeno-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="6d46e-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="6d46e-108">več</span><span class="sxs-lookup"><span data-stu-id="6d46e-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

