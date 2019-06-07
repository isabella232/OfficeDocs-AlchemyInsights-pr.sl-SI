---
title: Popraviti DKIM nastavljanjem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765417"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="c3187-102">Popraviti DKIM nastavljanjem</span><span class="sxs-lookup"><span data-stu-id="c3187-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="c3187-103">Če imate vprašanja, ki omogočajo DKIM za domeno po meri, sledite naslednjim korakom:</span><span class="sxs-lookup"><span data-stu-id="c3187-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="c3187-104">Večina DKIM namestitev vprašanja so povezana z napačne zapise DNS.</span><span class="sxs-lookup"><span data-stu-id="c3187-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="c3187-105">Preverite, ali zapis DKIM CNAME (**ne** zapis TXT) pravilno oblikovana.</span><span class="sxs-lookup"><span data-stu-id="c3187-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="c3187-106">Če želite več informacij, glejte to [temo](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="c3187-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="c3187-107">Ko ustvarite ali posodobiti vaše DKIM DNS zapisov na DNS sovražen usluga za domeno (praviloma svojega registratorja domene), čakati na zapise DNS, da širi.</span><span class="sxs-lookup"><span data-stu-id="c3187-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="c3187-108">Če ne morete ustvariti DKIM DNS zapisov v skrbniškem središču, lahko zamenjate \<CustomDomain\> z domeno po meri (na primer contoso.com) in zaženite ta ukaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="c3187-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
