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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407366"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="976b8-102">Primarnega e-poštnega naslova ni mogoče nastaviti, spremeniti uporabniških atributov ali odstraniti/izbrisati sinhroniziranega uporabnika</span><span class="sxs-lookup"><span data-stu-id="976b8-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="976b8-103">Če je sinhronizacija imenika omogočena za vaše okolje, nekaterih atributov uporabnika ali predmeta ni mogoče spremeniti s skrbniškim središčem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="976b8-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="976b8-104">Če želite v celoti upravljati sinhronizirane uporabnike in vse njihove atribute, uporabite lokalne uporabnike imenika Active Directory in konzolo za upravljanje skupin (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="976b8-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="976b8-105">Lahko pa tudi spremenite posamezne uporabnike ali atribute za sinhronizirane uporabnike z lupino, kot je prikazano v teh pogostih primerih:</span><span class="sxs-lookup"><span data-stu-id="976b8-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
