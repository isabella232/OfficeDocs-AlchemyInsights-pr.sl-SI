---
title: 'AIP: pravilniki, ki se ne obnašajo po pričakovanjih'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663205"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="ab3ca-102">AIP: pravilniki, ki se ne obnašajo po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="ab3ca-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="ab3ca-103">Zaščita informacij Azure: pravilniki, ki se ne obnašajo po pričakovanjih, si oglejte navodila za priporočene smernice za različne težave pravilnika:</span><span class="sxs-lookup"><span data-stu-id="ab3ca-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="ab3ca-104">Če imate težave z vizualnimi oznakami, si oglejte, [Kdaj se izvajajo vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="ab3ca-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="ab3ca-105">Če imate težave s samodejnim označevanjem, si oglejte [navodila za konfiguracijo pogojev za samodejno in priporočeno razvrstitev za zaščito informacij](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) v storitvi Azure in informacije, [ki jih](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)iščejo.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="ab3ca-106">Če imate težave s storitvijo native/Pfile Protection, preberite [Konfiguracija datoteke API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="ab3ca-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="ab3ca-107">Preverite, ali uporabljate pravilnike o obsegu, ki niso pravilno konfigurirani: [kako konfigurirati pravilnik o varstvu informacij Azure za določene uporabnike z uporabo pravilnikov o obsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="ab3ca-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="ab3ca-108">Če Samodejna oznaka za Outlook ne deluje v Outlooku, ko priložite označen dokument, preverite, ali DRMEncryptProperty ni opredeljen, kot je opisano tukaj: [nastavitve registra IRM za varnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="ab3ca-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="ab3ca-109">Če še vedno prihaja do težav, si oglejte dnevnike odjemalca za zaščito informacij Azure in priložite izvožene dnevnike tej vstopnici.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="ab3ca-110">Odprite Officeov dokument ali ustvarite novo e-poštno sporočilo v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="ab3ca-111">Kliknite pomoč za **zaščito/občutljivost**  >  **in povratne informacije**.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="ab3ca-112">Kliknite **Izvozi dnevnike**.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="ab3ca-113">Shranite dnevnike na izbrano mesto in jih priložite na to zahtevo storitve.</span><span class="sxs-lookup"><span data-stu-id="ab3ca-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="ab3ca-114">Dodatni viri:</span><span class="sxs-lookup"><span data-stu-id="ab3ca-114">Additional resources:</span></span>

- [<span data-ttu-id="ab3ca-115">Konfiguracija oznake za vizualne oznake za zaščito informacij v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="ab3ca-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="ab3ca-116">Pregled dokumentacije za zaščito informacij Azure</span><span class="sxs-lookup"><span data-stu-id="ab3ca-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="ab3ca-117">Uporaba oznak občutljivosti v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ab3ca-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

