---
title: Exchange PowerShell in opustitev osnovnega preverjanja pristnosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813488"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="2eae8-102">Exchange PowerShell in opustitev osnovnega preverjanja pristnosti</span><span class="sxs-lookup"><span data-stu-id="2eae8-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="2eae8-103">Za najnovejše informacije o tem, kako se lahko povežete z lupino Exchange Online PowerShell brez uporabe osnovnega preverjana pristnosti, [glejte tukaj](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="2eae8-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="2eae8-104">Modul Windows PowerShell V2 ne uporablja osnovnega preverjanja pristnosti.</span><span class="sxs-lookup"><span data-stu-id="2eae8-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="2eae8-105">Upoštevajte, da morate kljub temu omogočiti osnovno preverjanje pristnosti v odjemalskem računalniku.</span><span class="sxs-lookup"><span data-stu-id="2eae8-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="2eae8-106">Novi modul PowerShell V2 uporablja sodobno preverjanje pristnosti za vzpostavljanje povezave za omogočanje vseh ukazov »cmdlet« za V2, ki temeljijo na protokolu REST.</span><span class="sxs-lookup"><span data-stu-id="2eae8-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="2eae8-107">Z ukazi »cmdlet« za V2 lahko dostopate tudi do starejših ukazov »cmdlet« za oddaljeni PowerShell (RPS), zaradi česar morate zagnati sejo oddaljenega ogrodja PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2eae8-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="2eae8-108">Če želite zagnati sejo RPS v računalniku s sistemom Windows, mora biti omogočeno osnovno preverjanje pristnosti WinRM v odjemalskem računalniku, čeprav modul preverja pristnost storitve z mehanizmom za sodobno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="2eae8-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="2eae8-109">Cevovod osnovnega preverjanja pristnosti WinRM se uporablja za posredovanje žetonov za sodobno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="2eae8-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="2eae8-110">Če je osnovno preverjanje pristnosti WinRM onemogočeno v odjemalskem računalniku, novi ukazi »cmdlet« za V2 še naprej delujejo (medtem ko starejši ukazi »cmdlet« za RPS ne delujejo več).</span><span class="sxs-lookup"><span data-stu-id="2eae8-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
