---
title: 646 kako nastaviti AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779527"
---
# <a name="configure-sync-features"></a><span data-ttu-id="81460-102">Nastavitev sinhronizacije funkcij</span><span class="sxs-lookup"><span data-stu-id="81460-102">Configure sync features</span></span>

<span data-ttu-id="81460-103">Sinje AD Connect vključuje številne funkcije, ki so privzeto omogočen, ali ki lahko kasneje.</span><span class="sxs-lookup"><span data-stu-id="81460-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="81460-104">Nekatere funkcije zahtevajo dodatno konfiguracijo v posebnih okoljih.</span><span class="sxs-lookup"><span data-stu-id="81460-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="81460-105">[Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) omejitev predmetov sinhronizirajo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="81460-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="81460-106">Privzeto, vsi uporabniki, stike, skupine, in Windows 10 računov računalnika sinhronizirajo.</span><span class="sxs-lookup"><span data-stu-id="81460-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="81460-107">Lahko vključujejo ali izključujejo predmete, ki temeljijo na domene, OU-ji, ali druge lastnosti.</span><span class="sxs-lookup"><span data-stu-id="81460-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="81460-108">[Parola haše sinhronizacija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizira geslo haše iz krajevnega imenika Active Directory za modro AD.</span><span class="sxs-lookup"><span data-stu-id="81460-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="81460-109">To omogoča upravljanje gesel na enem mestu, ampak uporabite isto geslo krajevnimi in oblak okoljih.</span><span class="sxs-lookup"><span data-stu-id="81460-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="81460-110">Ker aktivni imenik je avtoritativni vir, lahko uporabite svoje pravilnike za gesla.</span><span class="sxs-lookup"><span data-stu-id="81460-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="81460-111">[Samopostrežno parola prikrivati (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogučiti uporabnik v prikrivati svoja gesla v oblaku, medtem ko še vedno uporabi pravilnik za gesla krajevne.</span><span class="sxs-lookup"><span data-stu-id="81460-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="81460-112">[Writeback naprava](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogoča registrirani naprav v sinje oglas za pisanje nazaj na imeniku Active Directory, se lahko uporabijo za pogojni dostop.</span><span class="sxs-lookup"><span data-stu-id="81460-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="81460-113">[Preprečevanje nenamernega izbriše](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočen za pomoč pri preprečevanju preveč sočasno predmet Izbrisi (več kot 500 predmetov na sinhronizacijo).</span><span class="sxs-lookup"><span data-stu-id="81460-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="81460-114">Spremenite lahko te nastavitve za potrebe vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="81460-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="81460-115">[Samodejno nadgradnjo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je privzeto omogočen za hitre naprave in pomaga zagotoviti vašo različico Azure AD povezavo je vedno Trenutna.</span><span class="sxs-lookup"><span data-stu-id="81460-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

