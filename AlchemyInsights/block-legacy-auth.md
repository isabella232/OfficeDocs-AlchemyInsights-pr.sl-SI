---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685614"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="9e1a5-102">Blokiranje podedovanega preverjanja pristnosti</span><span class="sxs-lookup"><span data-stu-id="9e1a5-102">Blocking legacy authentication</span></span>

<span data-ttu-id="9e1a5-103">Podedovano preverjanje pristnosti je izraz, ki se sklicuje na zahtevo za preverjanje pristnosti, ki jo je naredila:</span><span class="sxs-lookup"><span data-stu-id="9e1a5-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="9e1a5-104">Starejše Officeove odjemalce, ki ne uporabljajo sodobnega preverjanja pristnosti (na primer odjemalec za Office 2010).</span><span class="sxs-lookup"><span data-stu-id="9e1a5-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="9e1a5-105">Kateri koli odjemalec, ki uporablja podedovane poštne protokole, kot je IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="9e1a5-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="9e1a5-106">Če želite več informacij o blokiranju podedovanega preverjanja pristnosti in omogočanju sodobnega preverjanja pristnosti, glejte [blokiranje podedovanega preverjanja pristnosti](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="9e1a5-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="9e1a5-107">Varnostne privzete nastavitve v imeniku Azure Active Directory (Azure AD) Poenostavite varnost in zaščitite svojo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="9e1a5-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="9e1a5-108">Varnostne privzete vrednosti vsebujejo vnaprej konfigurirane varnostne nastavitve za pogoste napade.</span><span class="sxs-lookup"><span data-stu-id="9e1a5-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="9e1a5-109">Če želite več informacij o varnostnih privzetih nastavitvah, glejte [Kaj so privzete nastavitve varnosti?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="9e1a5-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="9e1a5-110">**Opomba**: če je bil vaš najemnik ustvarjen na ali po 22 oktober 2019, je morda prišlo do novega varnega obnašanja in že imate omogočene varnostne nastavitve v najemniku.</span><span class="sxs-lookup"><span data-stu-id="9e1a5-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="9e1a5-111">V želji, da zaščitite vse uporabnike, se varnostne privzete nastavitve izvlečejo v vse nove ustvarjene najemnike.</span><span class="sxs-lookup"><span data-stu-id="9e1a5-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
