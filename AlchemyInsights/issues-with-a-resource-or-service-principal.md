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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714460"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Težave z glavnim virom ali storitvijo

1. Če ste šele začeli [uporabljati glavne predmete aplikacije in storitve v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) , je v imeniku Azure Active Directory opisana registracija programov, predmeti aplikacije in upravniki storitev v imeniški storitvi, ki jih uporabljajo in kako so povezani s seboj. Predstavljen je tudi primer scenarija multi-najemnika, ki ponazarja razmerje med predmetom aplikacije in pripadajočimi glavnimi predmeti storitve.
2. Več informacij o relacijah med programi in glavnimi storitvami najdete v članku branje [aplikacij in osnovnih predmetov storitve v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Kako: uporabite portal za ustvarjanje aplikacije AZURE ad in glavnice storitve, ki lahko dostopajo do virov](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) , vam pokaže, kako ustvarite nov program za uporabo storitve Azure Active Directory (Azure ad), ki ga je mogoče uporabiti s kontrolnikom za dostop, ki temelji na vlogi.
4. S [storitvijo glavnega vmesnika API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)lahko programsko upravljate primerke programov in nadzorujete, kaj lahko stori aplikacija v najemniku.
5. [servicePrincipal vrsta vira](https://docs.microsoft.com/graph/api/resources/serviceprincipal) prikaže seznam vseh lastnosti in načinov za vrsto vira servicePrincipal.
6. [Razlike med vrstami virov med grafikonom AZURE ad Graph in programom Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) osvetljujejo razlike med Grafikonoma Azure ad Graph in viri Microsoft Graph. Prikazuje vire, ki imajo različna imena ali pa niso na voljo; izpostavlja tudi vire, ki so na voljo v različici beta programa Microsoft Graph, vendar ne v različici v 1.0.

**Težave z gostujočimi Uporabniki**

- [Hitri začetek: dodajanje gostujočih uporabnikov v imenik v portalu Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vam pokaže, kako dodate novega gostujočega uporabnika v imenik Azure ad prek portala Azure, pošljete povabilo in preverite, kako je videti postopek odkupa povabila gostujočega uporabnika.
- [Vadnica: ustvarjanje tokov uporabnikov v storitvi Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) vam pokaže, kako ustvarite priporočene uporabniške tokove s portalom Azure. Če iščete informacije o tem, kako nastavite vir poverilnic za gesla za lastnike virov (ROPC) v aplikaciji, si oglejte konfiguracija poverilnic za gesla za lastnike virov v storitvi Azure AD B2C.
