---
title: 'AIP: politike, ki se ne obnaša po pričakovanjih'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506574"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="6c5f6-102">AIP: politike, ki se ne obnaša po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="6c5f6-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="6c5f6-103">Azure Information Protection: pravilniki se ne obnaša po pričakovanjih, za priporočene smernice za različna politična vprašanja glejte naslednje:</span><span class="sxs-lookup"><span data-stu-id="6c5f6-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="6c5f6-104">Če imate težave z vizualnimi oznakami, preglejte, [Kdaj se uporabljajo vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="6c5f6-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="6c5f6-105">Če imate težave z avtomatskim označevanjem, preglejte, [Kako konfigurirate pogoje za samodejno in priporočeno razvrščanje za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) in [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="6c5f6-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="6c5f6-106">Če imate težave z native/Pfile zaščito, prosimo, preglejte [datoteko API konfiguracijo](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="6c5f6-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="6c5f6-107">Preverite, ali uporabljate pravilnike v obsegu, ki niso pravilno konfigurirani: [kako konfigurirati pravilnik o varstvu podatkov Azure za določene uporabnike z uporabo pravilnikov v obsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="6c5f6-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="6c5f6-108">Če samodejno označevanje ne deluje v Outlooku, ko pripnete označeni dokument, preverite, ali DRMEncryptProperty ni definiran, kot je opisano tukaj: [nastavitve registra IRM za varnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="6c5f6-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="6c5f6-109">Če še vedno naletite na težave, prosimo, zberite Azure Information Protection dnevniki in priložite izvožene dnevnike na to vozovnico.</span><span class="sxs-lookup"><span data-stu-id="6c5f6-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="6c5f6-110">Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="6c5f6-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="6c5f6-111">Kliknite **zaščitite/občutljivost**  >  **pomoč in povratne informacije**.</span><span class="sxs-lookup"><span data-stu-id="6c5f6-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="6c5f6-112">Kliknite **Izvozi dnevnike**.</span><span class="sxs-lookup"><span data-stu-id="6c5f6-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="6c5f6-113">Shranite dnevnike na svojo izbiro lokacije in jih priložite tej zahtevi za storitev.</span><span class="sxs-lookup"><span data-stu-id="6c5f6-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="6c5f6-114">Dodatni viri:</span><span class="sxs-lookup"><span data-stu-id="6c5f6-114">Additional resources:</span></span>

- [<span data-ttu-id="6c5f6-115">Konfiguriranje oznake za vizualne oznake za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6c5f6-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="6c5f6-116">Preglejte dokumentacijo o varstvu podatkov Azure</span><span class="sxs-lookup"><span data-stu-id="6c5f6-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="6c5f6-117">Uporaba oznak občutljivosti v Officeovih aplikacijah</span><span class="sxs-lookup"><span data-stu-id="6c5f6-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

