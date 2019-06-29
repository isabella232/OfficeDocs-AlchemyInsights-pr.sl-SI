---
title: Upravljanje sinhroniziranega uporabnika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380521"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="6d3fd-102">Ni mogoče nastaviti primarni e-poštni naslov ali spremenite atribute</span><span class="sxs-lookup"><span data-stu-id="6d3fd-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="6d3fd-103">Če je omogočena sinhronizacija imenika za vaš okolja ni mogoče spremeniti nekaterih atributov uporabnika ali predmet, z uporabo Admin Center.</span><span class="sxs-lookup"><span data-stu-id="6d3fd-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="6d3fd-104">Da v celoti upravljati sinhronizirani uporabniki in njihove lastnosti, uporabite vaš lokalni imenik active directory uporabniki in skupine konzolo za upravljanje (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="6d3fd-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="6d3fd-105">Alternativno, lahko spremenite posamezne uporabnike ali atributi za sinhronizirani uporabniki z uporabo powershell, kot je prikazano v teh pogosti primeri:</span><span class="sxs-lookup"><span data-stu-id="6d3fd-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="6d3fd-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6d3fd-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="6d3fd-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testni uporabnik" - priimek "Uporabnik"-naslov "Manager"-oddelek "HR"</span><span class="sxs-lookup"><span data-stu-id="6d3fd-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="6d3fd-108">Odstrani-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6d3fd-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>