---
title: Sinhronizacija gesel za gesla za storitev Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177621"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="633ae-102">Sinhronizacija gesel za gesla za storitev Domain</span><span class="sxs-lookup"><span data-stu-id="633ae-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="633ae-103">**Če je vaš primerek Azure AD DS nastavljen tako, da omogočite sinhronizacijo z geslom**</span><span class="sxs-lookup"><span data-stu-id="633ae-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="633ae-104">Naletite na scenarij, v katerem izvajate hibridno okolje z uporabniki, ki se sinhronizirajo z okoljem domenskih storitev Azure Active Directory (AD DS) na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="633ae-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="633ae-105">Ta postopek je naletel, kljub temu, da imate na mestu AD DS na mestu uporabe možnost sinhronizacije gesla, s svojim najemnikom storitve Azure AD.</span><span class="sxs-lookup"><span data-stu-id="633ae-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="633ae-106">**Ker**</span><span class="sxs-lookup"><span data-stu-id="633ae-106">**Cause**</span></span>

<span data-ttu-id="633ae-107">To se dogaja, ker Azure AD Connect by default ne sinhronizira podedovane nove tehnologije LAN upravitelja (NTLM) in Kerberos password, ki so potrebni za Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="633ae-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="633ae-108">**Rešitev**</span><span class="sxs-lookup"><span data-stu-id="633ae-108">**Workaround**</span></span> 

<span data-ttu-id="633ae-109">Če želite sinhronizirati gesla, potrebna za preverjanje pristnosti protokola NTLM in Kerberos, morate konfigurirati povezavo s storitvijo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="633ae-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="633ae-110">Ko je konfiguracija storitve Azure AD Connect konfigurirana, se ustvari račun na mestu uporabe ali dogodek spremembe gesla, nato pa sinhronizira podedovano geslo v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="633ae-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="633ae-111">Če želite več informacij o tem in navodila za omogočanje sinhronizacije gesel v hibridnih okoljih storitve Azure AD DS, si oglejte [tukaj](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) .</span><span class="sxs-lookup"><span data-stu-id="633ae-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>