---
title: Težave z glavnim virom ali storitvijo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028092"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Težave z glavnim virom ali storitvijo

1. Če ste šele začeli, glavni predmeti programa in storitve v programu Azure Active Directory opisujejo registracijo aplikacije, predmete programa in glavna vprašanja storitve v storitvi Azure Active Directory: kaj so, kako jih uporabljate [in](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) kako so med seboj povezani. Predstavljen je tudi primer z več najemniki, ki prikazuje razmerje med predmetom aplikacije in pripadajočimi glavnimi predmeti storitve.
2. Več o odnosu med programi in glavnimi predmeti storitve lahko izveste v programih in glavnih [predmetih storitve v Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Navodila:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) S portalom ustvarite glavno ime aplikacije in storitve Azure AD, ki lahko dostopa do virov, je prikazano, kako ustvarite novo aplikacijo in glavno ime storitve Azure Active Directory (Azure AD), ki ga lahko uporabljate s kontrolnikom za dostop na osnovi vloge.
4. Z [glavnim API-jem](https://docs.microsoft.com/graph/api/resources/serviceprincipal)storitve lahko programsko upravljate primerke aplikacij in nadzorujete, kaj lahko aplikacija naredi v najemniku.
5. [servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.
6. [Razlike med viri med viri Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) in Microsoft Graph med viri Azure AD Graph in Microsoft Graph. Prikazuje vire z različnimi imeni ali pa niso na voljo; prav tako označi vire, ki so na voljo v različici beta programa Microsoft Graph vendar ne v različici v1.0.

**Težave z gostuimi uporabniki**

- [Hitri začetek:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Dodajanje gostužnih uporabnikov v imenik v portalu Azure vam pokaže, kako dodate novega gostujočega uporabnika v imenik Azure AD prek portala Azure, pošljete povabilo in si ogledate, kako je videti postopek za unovčenje povabila gostužnega uporabnika.
- [Vadnica: ustvarjanje potekov uporabnikov v storitvi Azure Active Directory V2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) je prikazano, kako ustvarite priporočene uporabniške tokove s portalom Azure. Če želite informacije o tem, kako nastavite tok gesla lastnika vira v aplikaciji, glejte Konfiguracija toka poverilnic lastnika vira v storitvi Azure AD B2C.
