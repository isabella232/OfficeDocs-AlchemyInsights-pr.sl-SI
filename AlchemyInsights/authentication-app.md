---
title: Aplikacija za preverjanje pristnosti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405681"
---
# <a name="authentication-app"></a><span data-ttu-id="478e6-102">Aplikacija za preverjanje pristnosti</span><span class="sxs-lookup"><span data-stu-id="478e6-102">Authentication app</span></span>

<span data-ttu-id="478e6-103">Če ste globalni skrbnik, lahko z orodjem Diagnostika vpisa hitro ugotovite, kaj se je zgodilo, ali diagnosticirate težave, povezane z [vpisom uporabnika.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="478e6-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="478e6-104">Diagnostiko začnete tako, da kliknete gumb[»Zaženi diagnostiko«.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="478e6-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="478e6-105">Poiščite dogodek, ki ga želite analizirati, tako da vnesete podrobnosti o uporabniku, aplikaciji, času vpisa, ID-ju zahteve ali ID-ju korelacije.</span><span class="sxs-lookup"><span data-stu-id="478e6-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="478e6-106">Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko naredite za spreminjanje, če so potrebne spremembe.</span><span class="sxs-lookup"><span data-stu-id="478e6-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="478e6-107">**Preverite scenarij, ki velja:**</span><span class="sxs-lookup"><span data-stu-id="478e6-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="478e6-108">Če uporabnik ne dobiva potisnega obvestila v aplikaciji Microsoft Authenticator, preverite, ali niso prikazani pod blokiranimi uporabniki storitve MFA, kot je opisano v razdelku Blokiranje in [deblokiranje uporabnikov.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="478e6-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="478e6-109">Če uporabnik ni blokiran zaradi storitve MFA, vendar ne prejme potisnega obvestila, lahko odpre aplikacijo Microsoft Authenticator, ki povleče čakajoče zahteve za odobritev.</span><span class="sxs-lookup"><span data-stu-id="478e6-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="478e6-110">Uporabnik lahko kot alternativni način vpisa klikne tudi Vpis na drug način in izbere način uporabe kode za preverjanje iz moje mobilne aplikacije.</span><span class="sxs-lookup"><span data-stu-id="478e6-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="478e6-111">Aplikacija Microsoft Authenticator je edini na voljo za številne uporabnike.</span><span class="sxs-lookup"><span data-stu-id="478e6-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="478e6-112">[Več informacij o privzetih varnostnih nastavitvamih](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)najdete v članku Pogosta vprašanja o aplikaciji [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) za pogosta vprašanja in kako jih odpravite.</span><span class="sxs-lookup"><span data-stu-id="478e6-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="478e6-113">**Priporočeni videoposnetki**</span><span class="sxs-lookup"><span data-stu-id="478e6-113">**Recommended Videos**</span></span>

<span data-ttu-id="478e6-114">[Nastavitev aplikacije Authenticator v novem telefonu (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="478e6-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
