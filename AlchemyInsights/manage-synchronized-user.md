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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542020"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="d0478-102">Ni mogoče nastaviti primarni e-poštni naslov ali spremenite atribute</span><span class="sxs-lookup"><span data-stu-id="d0478-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="d0478-103">Če sinhronizacija imenika omogočena za vaše okolje, ni mogoče spremeniti nekaterih atributov uporabnika ali predmet, z uporabo Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="d0478-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="d0478-104">Da v celoti upravljati sinhronizirani uporabniki in njihove lastnosti, uporabite vaš lokalni imenik active directory uporabniki in skupine konzolo za upravljanje (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="d0478-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="d0478-105">Alternativno, lahko spremenite posamezne uporabnike ali atributi za sinhronizirani uporabniki z uporabo powershell, kot je prikazano v teh pogosti primeri:</span><span class="sxs-lookup"><span data-stu-id="d0478-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="d0478-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d0478-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="d0478-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testni uporabnik" - priimek "Uporabnik"-naslov "Manager"-oddelek "HR"</span><span class="sxs-lookup"><span data-stu-id="d0478-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="d0478-108">Odstrani-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d0478-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>