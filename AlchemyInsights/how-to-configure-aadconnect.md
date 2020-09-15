---
title: 646 kako konfigurirate AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704505"
---
# <a name="configure-sync-features"></a><span data-ttu-id="abe54-102">Konfiguracija funkcij sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="abe54-102">Configure sync features</span></span>

<span data-ttu-id="abe54-103">V storitvi Azure AD Connect so na voljo številne funkcije, ki so privzeto omogočene ali pa jih lahko omogočite pozneje.</span><span class="sxs-lookup"><span data-stu-id="abe54-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="abe54-104">Nekatere funkcije zahtevajo dodatno konfiguracijo v določenih okoljih.</span><span class="sxs-lookup"><span data-stu-id="abe54-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="abe54-105">Omejitve [filtriranja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) predmeti se sinhronizirajo s storitvijo Azure ad.</span><span class="sxs-lookup"><span data-stu-id="abe54-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="abe54-106">Privzeto so vsi uporabniki, stiki, skupine in računi v računalniku s sistemom Windows 10 sinhronizirani.</span><span class="sxs-lookup"><span data-stu-id="abe54-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="abe54-107">Predmete lahko vključite ali izključite na osnovi domen, organizacijskih ali drugih atributov.</span><span class="sxs-lookup"><span data-stu-id="abe54-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="abe54-108">[Sinhronizacija gesla za razprševanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizira geslo razpršitve iz imenika Active Directory na mestu uporabe v storitvi Azure ad.</span><span class="sxs-lookup"><span data-stu-id="abe54-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="abe54-109">S tem lahko upravljate upravljanje gesel na enem mestu, vendar uporabite enako geslo v okoljih na mestu uporabe in v oblaku.</span><span class="sxs-lookup"><span data-stu-id="abe54-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="abe54-110">Ker je Active Directory avtoritativni vir, lahko uporabite svoje pravilnike za gesla.</span><span class="sxs-lookup"><span data-stu-id="abe54-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="abe54-111">[Samopostrežno ponastavitev gesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) uporabnikom omogoča, da ponastavijo svoja gesla v oblaku, medtem ko še vedno uporabljajo pravilnike za gesla na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="abe54-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="abe54-112">[Naprava nepotrjenim](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogoča, da se registrirane naprave v storitvi Azure ad zapišejo v imenik Active Directory na mestu uporabe, da jih je mogoče uporabiti za pogojni dostop.</span><span class="sxs-lookup"><span data-stu-id="abe54-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="abe54-113">[Preprečevanje nenamernih brisanj](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočeno, da preprečite preveč hkratnih brisanj predmetov (več kot 500 predmetov na sinhronizacijo).</span><span class="sxs-lookup"><span data-stu-id="abe54-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="abe54-114">To nastavitev lahko spremenite, da zadovoljite potrebe organizacije.</span><span class="sxs-lookup"><span data-stu-id="abe54-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="abe54-115">[Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je privzeto omogočena za ekspresne naprave in zagotavlja, da je različica storitve Azure ad Connect vedno aktualna.</span><span class="sxs-lookup"><span data-stu-id="abe54-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
