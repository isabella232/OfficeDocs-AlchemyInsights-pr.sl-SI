---
title: Imenik Active Directory se ne sinhronizira
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930991"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="968fe-102">Imenik Active Directory se ne sinhronizira</span><span class="sxs-lookup"><span data-stu-id="968fe-102">Active Directory not syncing</span></span>

<span data-ttu-id="968fe-103">Če prejemate napake pri sinhronizaciji, na primer »ni nedavne sinhronizacije«, ali pa opazite stanje sinhronizacije imenika v skrbniškem portalu za Office pravi »Zadnja sinhronizacija je bila sinhronizirana pred več kot 3 dnevi«, ima morda AADConnect nepravilne nastavitve ali nezadostna dovoljenja za izvajanje sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="968fe-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="968fe-104">Če znova namestite AADConnect s hitrimi nastavitvami, boste težavo morda lahko hitro odpravili:</span><span class="sxs-lookup"><span data-stu-id="968fe-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="968fe-105">[Prenesite najnovejšo različico programa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="968fe-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="968fe-106">[Upoštevajte navodila za hitro namestitev.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="968fe-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="968fe-107">Storitev Azure AD Connect mora biti nameščena v strežniku Windows Server 2012 ali novejši različici.</span><span class="sxs-lookup"><span data-stu-id="968fe-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="968fe-108">Ta strežnik mora biti pridružena domena in je lahko krmilnik domene oziroma članski strežnik.</span><span class="sxs-lookup"><span data-stu-id="968fe-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="968fe-109">Za celoten seznam zahtev in Povezovalnik imenika Azure AD si oglejte Zahteve za imenik [Azure AD Povezovalnik](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="968fe-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="968fe-110">Če želite več informacij o računih storitve AADConnect, glejte [Azure AD Povezovalnik: Računi in dovoljenja.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="968fe-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
