---
title: Težava z enim uporabnikom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430207"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="c234e-102">Težava z enim uporabnikom</span><span class="sxs-lookup"><span data-stu-id="c234e-102">Problem with single user</span></span>

- <span data-ttu-id="c234e-103">Uporabnik morda ni bil omogočen, ker storitev še ni imela možnosti, da bi ocenila uporabnika.</span><span class="sxs-lookup"><span data-stu-id="c234e-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="c234e-104">Preglejte navodila o tem, kako dolgo omogoča omogočanje uporabe, kot tudi vrstico napredovanja na strani s konfiguracijo za omogočanje uporabe.</span><span class="sxs-lookup"><span data-stu-id="c234e-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="c234e-105">Če je stanje stalnega stanja, ki je določeno v razdelku dodatne podrobnosti, pred datumom, ko je bil uporabnik ustvarjen/posodobljen/izbrisan, to pomeni, da še nismo ocenili uporabnika.</span><span class="sxs-lookup"><span data-stu-id="c234e-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="c234e-106">V tem primeru je najbolje, da počakate, da se storitev za omogočanje uporabe dokonča.</span><span class="sxs-lookup"><span data-stu-id="c234e-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="c234e-107">Upoštevajte, da je naša storitev seznanjena le s spremembami uporabnika v izvornem sistemu (v oblaku).</span><span class="sxs-lookup"><span data-stu-id="c234e-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="c234e-108">Obstajati mora veljavna sprememba v izvornem sistemu za Azure AD, da zazna spremembo in jo poteče v imenik Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c234e-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="c234e-109">Storitev za omogočanje uporabe je ocenila uporabnika in ga določila, da ne sme biti omogočena:</span><span class="sxs-lookup"><span data-stu-id="c234e-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="c234e-110">Če ste nastavili filter za določanje obsega na osnovi atributa, zagotovite, da uporabnik izpolnjuje pogoje, ki ste jih navedli.</span><span class="sxs-lookup"><span data-stu-id="c234e-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="c234e-111">Če uporabniki že obstajajo v ciljnem sistemu in stanju uporabnika v izvorni in ciljni tekmi, ne bomo ukrepali.</span><span class="sxs-lookup"><span data-stu-id="c234e-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="c234e-112">Storitev za omogočanje uporabe je poskušala omogočiti uporabnika in je spodletela.</span><span class="sxs-lookup"><span data-stu-id="c234e-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="c234e-113">Za te scenarije si oglejte zavihek odpravljanje težav in priporočil v dnevnikih za omogočanje uporabe:</span><span class="sxs-lookup"><span data-stu-id="c234e-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="c234e-114">Zahtevani atribut uporabnika morda manjka v imeniku Active Directory na mestu uporabe ali v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c234e-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c234e-115">Na primer pravila userPrincipalName ali sAMAccountName generacije ne ustvarijo prave vrednosti.</span><span class="sxs-lookup"><span data-stu-id="c234e-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="c234e-116">Ujemajoči se atribut (običajno IDZaposlenega) ne razreši enoličnemu uporabniku v imeniku Active Directory na mestu uporabe ali v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c234e-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c234e-117">Na primer obstajata dva uporabnika z istim IDZaposlenega v storitvi AD in storitev vrne kodo napake, ki označuje podvojene ciljne vnose za isti izvorni vnos.</span><span class="sxs-lookup"><span data-stu-id="c234e-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="c234e-118">Če želite pregledati dnevnike za enega uporabnika in skupine, si oglejte [pregled dnevnikov za omogočanje težave z določenim uporabnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="c234e-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
