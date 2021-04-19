---
title: Pravilniki o pogojnem dostopu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817296"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="66d6e-102">Pravilniki o pogojnem dostopu</span><span class="sxs-lookup"><span data-stu-id="66d6e-102">Conditional Access policies</span></span>

<span data-ttu-id="66d6e-103">Pogojni dostop je zmogljivost v storitvi Azure AD, ki omogoča uveljavitev kontrolnikov za dostop do aplikacije v svojem okolju – vse temelji na določenih pogojih in je upravljano z osrednjega mesta.</span><span class="sxs-lookup"><span data-stu-id="66d6e-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="66d6e-104">Več informacij o [pogojnem dostopu v storitvi Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="66d6e-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="66d6e-105">**Opomba**: če je bil vaš najemnik ustvarjen po 21. oktobru 2019 in nepričakovano prejmete poziv za večkratno preverjanje pristnosti, imate v svojem najemniku najverjetneje omogočene privzete [varnostne nastavitve](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="66d6e-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="66d6e-106">**Upravljanje privzetih varnostnih nastavitev**</span><span class="sxs-lookup"><span data-stu-id="66d6e-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="66d6e-107">Vpišite se v [skrbniško središče](https://go.microsoft.com/fwlink/p/?linkid=834822) s svojimi poverilnicami globalnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="66d6e-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="66d6e-108">Pojdite v razdelek [z lastnostmi storitve Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="66d6e-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="66d6e-109">Pri dnu strani kliknite **Upravljanje privzetih nastavitev varnosti**.</span><span class="sxs-lookup"><span data-stu-id="66d6e-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="66d6e-110">Kliknite **Da**, da omogočite privzete varnostne nastavitve, ali **Ne**, če želite privzete varnostne nastavitve onemogočiti.</span><span class="sxs-lookup"><span data-stu-id="66d6e-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
