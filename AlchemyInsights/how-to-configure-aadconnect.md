---
title: 646 kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722579"
---
# <a name="configure-sync-features"></a><span data-ttu-id="363e3-102">Konfiguracija funkcij sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="363e3-102">Configure sync features</span></span>

<span data-ttu-id="363e3-103">Azure AD Connect vključuje več funkcij, ki so privzeto omogočene, ali pa jih lahko pozneje omogočite.</span><span class="sxs-lookup"><span data-stu-id="363e3-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="363e3-104">Nekatere funkcije zahtevajo dodatno konfiguracijo v določenih okoljih.</span><span class="sxs-lookup"><span data-stu-id="363e3-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="363e3-105">[Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) omejuje, da so predmeti sinhronizirani s storitvijo Azure ad.</span><span class="sxs-lookup"><span data-stu-id="363e3-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="363e3-106">Privzeto se sinhronizirajo vsi uporabniki, stiki, skupine in računi računalnika s sistemom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="363e3-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="363e3-107">Predmete lahko vključite ali izključite na podlagi domen, OUs ali drugih atributov.</span><span class="sxs-lookup"><span data-stu-id="363e3-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="363e3-108">[Sinhronizacija za razprševanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) gesel sinhronizira razprševanje gesla iz krajevnega imenika Active Directory v Azure ad.</span><span class="sxs-lookup"><span data-stu-id="363e3-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="363e3-109">To omogoča upravljanje gesel na enem mestu, vendar Uporaba istega gesla v krajevnih in oblačnih okoljih.</span><span class="sxs-lookup"><span data-stu-id="363e3-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="363e3-110">Ker je Active Directory avtoritativni vir, lahko uporabite svoje pravilnike o geslih.</span><span class="sxs-lookup"><span data-stu-id="363e3-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="363e3-111">[Samopostrežna ponastavitev gesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogoča uporabnikom, da ponastavijo svoja gesla v oblaku, medtem ko še vedno uporabljajo krajevni pravilnik o geslih.</span><span class="sxs-lookup"><span data-stu-id="363e3-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="363e3-112">[Naprava writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogoča, da se registrirane naprave v storitvi Azure ad zapišemo nazaj v krajevni imenik Active Directory, tako da jih je mogoče uporabiti za pogojni dostop.</span><span class="sxs-lookup"><span data-stu-id="363e3-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="363e3-113">[Preprečite nenamerno brisanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je privzeto omogočeno, da se prepreči preveč hkratnih brisanja predmetov (več kot 500 predmetov na sinhronizacijo).</span><span class="sxs-lookup"><span data-stu-id="363e3-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="363e3-114">To nastavitev lahko spremenite tako, da ustreza potrebam vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="363e3-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="363e3-115">[Samodejna nadgradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je privzeto omogočena za hitre namestitve in pomaga zagotoviti, da je vaša različica Azure ad Connect vedno aktuna.</span><span class="sxs-lookup"><span data-stu-id="363e3-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
