---
title: 'AIP: Pravilniki se ne poshajo po pričakovanjih'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821643"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="a75d7-102">AIP: Pravilniki se ne poshajo po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="a75d7-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="a75d7-103">Azure Information Protection: Pravilniki se ne obnašajo po pričakovanjih. Če želite priporočene smernice za različne težave s pravilnikom, glejte te smernice:</span><span class="sxs-lookup"><span data-stu-id="a75d7-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="a75d7-104">Če imate težave z vizualnimi oznakami, preglejte [Ko uporabite vizualne oznake.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="a75d7-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="a75d7-105">Če imate težave s samodejnim označevanjem, preberite Konfiguracija pogojev za samodejno in priporočeno razvrstitev za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) in Kaj so vrste občutljivih [informacij.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a75d7-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="a75d7-106">Če imate težave z izvorno zaščito/zaščito datoteke Pfile, preglejte Konfiguracija [API-ja datoteke.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="a75d7-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="a75d7-107">Preverite, ali uporabljate pravilnike z obsegi, ki niso pravilno konfigurirani: Kako konfigurirati pravilnik Azure Information Protection za določene uporabnike z [uporabo pravilnikov o obsegu.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="a75d7-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="a75d7-108">Če samodejno označevanje ne deluje v Outlooku, ko priložite označen dokument, se prepričajte, da DRMEncryptProperty ni definiran tako, kot je opisano tukaj: Nastavitve registra upravljanja pravic do informacij za [varnost.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="a75d7-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="a75d7-109">Če še vedno prihaja do težav, zberite dnevnike odjemalcev za Azure Information Protection in priložite izvožene dnevnike tej vstopnici.</span><span class="sxs-lookup"><span data-stu-id="a75d7-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="a75d7-110">Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="a75d7-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="a75d7-111">Kliknite **Pomoč za zaščito/občutljivost**  >  **in povratne informacije.**</span><span class="sxs-lookup"><span data-stu-id="a75d7-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="a75d7-112">Kliknite **Izvoz dnevnikov.**</span><span class="sxs-lookup"><span data-stu-id="a75d7-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="a75d7-113">Shranite dnevnike v svojo izbiro lokacije in jih priložite tej zahtevi za storitev.</span><span class="sxs-lookup"><span data-stu-id="a75d7-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="a75d7-114">Dodatni viri:</span><span class="sxs-lookup"><span data-stu-id="a75d7-114">Additional resources:</span></span>

- [<span data-ttu-id="a75d7-115">Konfiguracija oznake za vizualne oznake za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a75d7-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="a75d7-116">Pregled dokumentacije Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a75d7-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="a75d7-117">Uporaba oznak občutljivosti v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a75d7-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

