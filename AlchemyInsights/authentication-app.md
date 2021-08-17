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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082958"
---
# <a name="authentication-app"></a>Aplikacija za preverjanje pristnosti

Če ste globalni skrbnik, lahko z orodjem Diagnostika vpisa hitro ugotovite, kaj se je zgodilo, ali diagnosticirate težave, povezane z [vpisom uporabnika.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Diagnostiko začnete tako, da kliknete gumb[»Zaženi diagnostiko«.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Poiščite dogodek, ki ga želite analizirati, tako da vnesete podrobnosti o uporabniku, aplikaciji, času vpisa, ID-ju zahteve ali ID-ju korelacije.
1. Preglejte diagnostične rezultate, ki prikazujejo podrobnosti o tem, kaj se je zgodilo in katera dejanja lahko naredite za spreminjanje, če so potrebne spremembe.

**Preverite scenarij, ki velja:**

1. Če uporabnik ne dobiva potisnega obvestila v aplikaciji Microsoft Authenticator, preverite, ali niso prikazani pod blokiranimi uporabniki storitve MFA, kot je opisano v razdelku Blokiranje in deblokiranje [uporabnikov.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Če uporabnik ni blokiran zaradi storitve MFA, vendar ne prejme potisnega obvestila, lahko odpre aplikacijo Microsoft Authenticator, ki bo povleče čakajoče zahteve za odobritev.
1. Uporabnik lahko kot alternativni način vpisa klikne tudi Vpis na drug način in izbere način uporabe kode za preverjanje iz moje mobilne aplikacije.
1. Aplikacija Microsoft Authenticator je edini način, ki je na voljo za številne uporabnike. [Več informacij o privzetih varnostih preberite](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [Authenticator pogostih](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) vprašanjih o aplikacijah in kako jih odpravite.
 
**Priporočeni videoposnetki**

[Kako nastavite aplikacijo Authenticator v novem telefonu (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
