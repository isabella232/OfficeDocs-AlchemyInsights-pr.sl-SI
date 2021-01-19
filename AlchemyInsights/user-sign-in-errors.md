---
title: Napake pri vpisu uporabnika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901253"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="c9dcf-102">Napake pri vpisu uporabnika</span><span class="sxs-lookup"><span data-stu-id="c9dcf-102">User sign-in errors</span></span>

<span data-ttu-id="c9dcf-103">**Odpravljanje težav z diagnostičnim vpisom**</span><span class="sxs-lookup"><span data-stu-id="c9dcf-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="c9dcf-104">Če želite zaznati težave, povezane z uporabniškim vpisom, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="c9dcf-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="c9dcf-105">Zaženite [diagnostiko za vpis](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="c9dcf-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="c9dcf-106">Poiščite dogodek, ki ga želite analizirati, tako da vnesete podrobnosti, ki jih imate o uporabniku, aplikaciji, času vpisa, zahtevi ID-ja ali korelaciji.</span><span class="sxs-lookup"><span data-stu-id="c9dcf-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="c9dcf-107">Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko izvedete, če želite spremeniti spremembe, če so potrebne spremembe.</span><span class="sxs-lookup"><span data-stu-id="c9dcf-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="c9dcf-108">**Iščete informacije o AADSTS kodah napak, ki so bile vrnjene v storitvi za varnost žetona Azure Active Directory ("Azure AD)" (STS)?**</span><span class="sxs-lookup"><span data-stu-id="c9dcf-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="c9dcf-109">Preberite [Ta članek](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , če želite poiskati AADSTS opise napak, popravke in nekatere predlagane rešitve</span><span class="sxs-lookup"><span data-stu-id="c9dcf-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>