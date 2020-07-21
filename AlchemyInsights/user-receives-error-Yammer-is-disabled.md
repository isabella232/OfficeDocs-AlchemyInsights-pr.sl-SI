---
title: Uporabnik prejme napako AADSTS7000112 Yammer je onemogočen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198371"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="4c937-102">Uporabnik prejme napako AADSTS7000112 Yammer je onemogočen</span><span class="sxs-lookup"><span data-stu-id="4c937-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="4c937-103">Če se prikaže napaka "AADSTS7000112: aplikacija" 00000005-0000-0ff1-CE00-000000000000 "(Yammer) je onemogočena", obstaja težava pri ravnatelju storitve v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c937-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="4c937-104">Skrbnik je morda onemogočil naročitelja storitev, da blokira dostop do storitve Yammer.</span><span class="sxs-lookup"><span data-stu-id="4c937-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="4c937-105">Onemogočanje glavnega servisa ni priporočeno in lahko povzroči dodatna vprašanja.</span><span class="sxs-lookup"><span data-stu-id="4c937-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="4c937-106">Če želite več informacij o podprtem pristopu za blokiranje uporabniškega dostopa do programa Yammer, glejte izklop [dostopa do storitev yammer za Microsoftove uporabnike 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="4c937-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="4c937-107">Če želite to težavo odpraviti v portalu Azure in obnoviti dostop uporabnikov do storitev Yammer:</span><span class="sxs-lookup"><span data-stu-id="4c937-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="4c937-108">Odprite stran Azure Active Directory in izberite **aplikacije podjetja** pod **Upravljaj** v levem podoknu za krmarjenje.</span><span class="sxs-lookup"><span data-stu-id="4c937-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="4c937-109">V iskalno polje vnesite **Office 365 Yammer** in izberite ime aplikacije, da odprete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="4c937-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="4c937-110">V levem podoknu za krmarjenje izberite **lastnosti** pod **Upravljaj** .</span><span class="sxs-lookup"><span data-stu-id="4c937-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="4c937-111">Nastavite vrednost **omogočenega za prijavo za uporabnike?** za **Yes**in nato izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="4c937-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="4c937-112">Znova se vpišite v Yammer.</span><span class="sxs-lookup"><span data-stu-id="4c937-112">Sign in to Yammer again.</span></span> <span data-ttu-id="4c937-113">Morda boste morali počistiti piškotke.</span><span class="sxs-lookup"><span data-stu-id="4c937-113">You might need to clear cookies.</span></span>

<span data-ttu-id="4c937-114">Izmeničen, prost dostop PowerShell zapoved v število enakih oseb vrednost.</span><span class="sxs-lookup"><span data-stu-id="4c937-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="4c937-115">Če želite več informacij, glejte ["Žal mi je, vendar imamo težave pri vpisu v" napako, ko kliknete ploščico Yammer v Officeu 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4c937-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 