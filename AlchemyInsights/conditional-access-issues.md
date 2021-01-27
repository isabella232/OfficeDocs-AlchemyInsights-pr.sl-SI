---
title: Težave s pogojnim dostopom
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015002"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="46556-102">Težave s pogojnim dostopom</span><span class="sxs-lookup"><span data-stu-id="46556-102">Conditional access issues</span></span>

<span data-ttu-id="46556-103">**Odpravljanje težav z diagnostičnim vpisom**</span><span class="sxs-lookup"><span data-stu-id="46556-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="46556-104">Hitro lahko ugotovite, kaj se je zgodilo ali diagnosticirali težave, povezane z uporabniškim vpisom, in sicer tako, da uporabite [diagnostično prijavo](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="46556-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="46556-105">Zaženite diagnostiko za vpis.</span><span class="sxs-lookup"><span data-stu-id="46556-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="46556-106">Poiščite dogodek, ki ga želite analizirati, in sicer tako, da vnesete podrobnosti o uporabniku, aplikaciji, času vpisa, ID-ju zahteve ali korelaciji.</span><span class="sxs-lookup"><span data-stu-id="46556-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="46556-107">Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko izvedete, če želite spremeniti (če so potrebne spremembe).</span><span class="sxs-lookup"><span data-stu-id="46556-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="46556-108">**Navodila za odpravljanje težav z vpisom**</span><span class="sxs-lookup"><span data-stu-id="46556-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="46556-109">Pomaknite se na stran za vpis v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="46556-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="46556-110">Vpisi filtra po uporabnikih, časovnem obsegu, aplikaciji, stanju, odjemalskem programu in tako dalje.</span><span class="sxs-lookup"><span data-stu-id="46556-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="46556-111">Izberite dogodek za vpis in si oglejte zavihek pogojni dostop, da si ogledate, katere pravilnike ste ocenili.</span><span class="sxs-lookup"><span data-stu-id="46556-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="46556-112">Kliknite vrstico pravilnika, če si želite ogledati podrobnosti pravilnika in razumeti, zakaj je uporabljen.</span><span class="sxs-lookup"><span data-stu-id="46556-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="46556-113">**Orodja za odpravljanje težav s pogojnim dostopom**</span><span class="sxs-lookup"><span data-stu-id="46556-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="46556-114">Način» samo za poročilo «vam omogoča, da ocenite pravilnik brez vpliva uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="46556-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="46556-115">Orodje» kaj-če «vam omogoča simulacijo dogodkov za vpis in ogled pravilnikov.</span><span class="sxs-lookup"><span data-stu-id="46556-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="46556-116">Delovni zvezek za vpoglede in poročanje prikaže sprotni vpliv posameznih pravilnikov.</span><span class="sxs-lookup"><span data-stu-id="46556-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="46556-117">**Pravilniki o zaščiti osnovnih podatkov**</span><span class="sxs-lookup"><span data-stu-id="46556-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="46556-118">Pravilniki o zaščiti po osnovnem načrtu so bili zastareli.</span><span class="sxs-lookup"><span data-stu-id="46556-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="46556-119">Niso več uveljavljene in bodo kmalu odstranjene iz portala Azure.</span><span class="sxs-lookup"><span data-stu-id="46556-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="46556-120">Priporočamo, da omogočite [varnostne privzete nastavitve](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="46556-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="46556-121">Če želite več informacij o pogojnem dostopu, glejte:</span><span class="sxs-lookup"><span data-stu-id="46556-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="46556-122">[Najboljši načini za pogojni dostop v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Pogoji v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolniki v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokacije v pogojnem dostopu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="46556-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
