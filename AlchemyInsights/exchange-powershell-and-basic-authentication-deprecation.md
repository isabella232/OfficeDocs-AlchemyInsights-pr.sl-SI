---
title: Exchange PowerShell in opustitev osnovnega preverjanja pristnosti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015705"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="f96b4-102">Exchange PowerShell in opustitev osnovnega preverjanja pristnosti</span><span class="sxs-lookup"><span data-stu-id="f96b4-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="f96b4-103">Za najnovejše informacije o tem, kako se lahko povežete z lupino Exchange Online PowerShell brez uporabe osnovnega preverjana pristnosti, [glejte tukaj](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="f96b4-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="f96b4-104">Upoštevajte, da morate kljub temu omogočiti osnovno preverjanje pristnosti v odjemalskem računalniku.</span><span class="sxs-lookup"><span data-stu-id="f96b4-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="f96b4-105">Novi modul PowerShell V2 uporablja sodobno preverjanje pristnosti za vzpostavljanje povezave za omogočanje vseh ukazov »cmdlet« za V2, ki temeljijo na protokolu REST.</span><span class="sxs-lookup"><span data-stu-id="f96b4-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="f96b4-106">Z ukazi »cmdlet« za V2 lahko dostopate tudi do starejših ukazov »cmdlet« za oddaljeni PowerShell (RPS), zaradi česar morate zagnati sejo oddaljenega ogrodja PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f96b4-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="f96b4-107">Če želite zagnati sejo RPS v računalniku s sistemom Windows, mora biti omogočeno osnovno preverjanje pristnosti WinRM v odjemalskem računalniku, čeprav modul preverja pristnost storitve z mehanizmom za sodobno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="f96b4-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="f96b4-108">Cevovod osnovnega preverjanja pristnosti WinRM se uporablja za posredovanje žetonov za sodobno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="f96b4-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="f96b4-109">Če je osnovno preverjanje pristnosti WinRM onemogočeno v odjemalskem računalniku, novi ukazi »cmdlet« za V2 še naprej delujejo (medtem ko starejši ukazi »cmdlet« za RPS ne delujejo več).</span><span class="sxs-lookup"><span data-stu-id="f96b4-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
