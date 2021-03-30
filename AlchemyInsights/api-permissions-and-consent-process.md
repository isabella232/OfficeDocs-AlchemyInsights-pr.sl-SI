---
title: Dovoljenja API in proces soglasja
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405441"
---
# <a name="api-permissions-and-consent-process"></a>Dovoljenja API in proces soglasja

Da bi vaša aplikacija lahko dostopala do podatkov v storitvi Microsoft Graph, ji mora uporabnik ali skrbnik prek postopka podelitve soglasja podeliti ustrezna dovoljenja. [Sklici dovoljenj za Microsoft Graph navajajo](https://docs.microsoft.com/graph/permissions-reference) dovoljenja, povezana z vsakim glavnim naborom API-jev za Microsoft Graph. V njem so na voljo tudi navodila za uporabo dovoljenj.

**Nastavljanje ali posodabljanje glavnega mesta storitve**

- [Ustvarjanje serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – v tem članku je prikazano, kako ustvarite nov predmet servicePrincipal.
- [Ustvarjanje glavnega imena aplikacije Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) glavnem imenu storitve na portalu – v tem članku je prikazano, kako ustvarite novo glavno ime aplikacije in storitve Azure Active Directory (Azure AD), ki jo lahko uporabljate z nadzorom dostopa na osnovi vloge.
- [Aplikacije &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) storitvah Azure AD – v tem članku so opisana registracija aplikacij, predmeti aplikacije in glavna imena storitev v imeniku Azure Active Directory: kaj so, kako jih uporabljate in kako so med seboj povezani.

**Dodajanje ali posodabljanje registracije aplikacije in zagotavljanje skrbniškega soglasja**

- [Ustvarite registracijo aplikacije –](https://docs.microsoft.com/graph/api/application-post-applications) v tem članku je prikazano, kako ustvarite nov predmet aplikacije.
- [Posodobitev registracije aplikacij – dovoljenja API-ja](https://docs.microsoft.com/graph/api/application-update) – v tem članku je prikazano, kako posodobite lastnosti predmeta aplikacije.
- [Zagotavljanje skrbniškega soglasja](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – za soglasje skrbnika in splošno soglasje potrebujemo, da skrbnik izrecno podeli soglasje.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – vsebnik upravljanja vlog za enotne definicije vlog in dodelitve vlog za ponudnike RBAC za Microsoft 365, ki podpirajo več glavnic in več obsegov pri eni dodelitvi vloge. Ta se razlikuje od *vrste vira rbacApplication.* Microsoft Intune je primer takšnega ponudnika za RBAC. Dodelitev vloge v intune ima lahko matriko glavnega mesta in obseg skupin. **To je v beta različici, kar pomeni, da je še vedno v razvoju in ga ne priporočamo za uporabo v produkciji.**
