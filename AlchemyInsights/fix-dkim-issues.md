---
title: Odpravljanje težav z nastavitvijo DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506790"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="66601-102">Odpravljanje težav z nastavitvijo DKIM</span><span class="sxs-lookup"><span data-stu-id="66601-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="66601-103">Če naletite na težave, ki omogočajo DKIM za vašo domeno po meri, uporabite naslednje korake:</span><span class="sxs-lookup"><span data-stu-id="66601-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="66601-104">Večina težav z nastavitvijo DKIM je povezanih z nepravilnimi zapisi DNS.</span><span class="sxs-lookup"><span data-stu-id="66601-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="66601-105">Preverite, ali je zapis DKIM CNAME (**ne** zapis txt) pravilno formatiran.</span><span class="sxs-lookup"><span data-stu-id="66601-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="66601-106">Če želite več informacij, glejte to [temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="66601-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="66601-107">Ko ustvarite ali posodobite zapise DKIM DNS v storitvi gostovanja DNS za vašo domeno (običajno je to registrar domene), počakajte, da se zapisi DNS razširijo.</span><span class="sxs-lookup"><span data-stu-id="66601-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="66601-108">Če v skrbniškem središču ne morete ustvariti zapisov DKIM DNS, lahko zamenjate \<CustomDomain\> z domeno po meri (na primer contoso.com) in zaženete ta ukaz v [PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="66601-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
