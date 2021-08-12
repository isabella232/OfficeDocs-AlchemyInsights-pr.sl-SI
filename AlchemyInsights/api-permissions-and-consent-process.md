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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932077"
---
# <a name="api-permissions-and-consent-process"></a>Dovoljenja API in proces soglasja

Če želite, da vaša aplikacija dostopa do podatkov v Graph Microsoft Graph, ji mora uporabnik ali skrbnik prek postopka podelitve soglasja podeliti ustrezna dovoljenja. [Microsoft Graph sklici dovoljenj naštejejo](https://docs.microsoft.com/graph/permissions-reference) dovoljenja, povezana z vsakim glavnim naborom API-jev Graph Microsoft. V njem so na voljo tudi navodila za uporabo dovoljenj.

**Nastavljanje ali posodabljanje glavnega mesta storitve**

- [Ustvarjanje serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – v tem članku je prikazano, kako ustvarite nov predmet servicePrincipal.
- [Ustvarjanje glavnega mesta storitve za & Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) na portalu – v tem članku je prikazano, kako ustvarite novo glavno ime aplikacije in storitve Azure Active Directory (Azure AD), ki jo lahko uporabljate s kontrolnikom za dostop na osnovi vloge.
- Aplikacije & glavnem imenu storitve v [Imeniku Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – v tem članku so opisana registracija aplikacije, predmeti aplikacije in glavnice storitve v programu Azure Active Directory: kaj so, kako jih uporabljate in kako so med seboj povezani.

**Dodajanje ali posodabljanje registracije aplikacije in zagotavljanje skrbniškega soglasja**

- [Ustvarite registracijo aplikacije –](https://docs.microsoft.com/graph/api/application-post-applications) v tem članku je prikazano, kako ustvarite nov predmet aplikacije.
- [Posodobitev registracije aplikacij – dovoljenja API-ja](https://docs.microsoft.com/graph/api/application-update) – v tem članku je prikazano, kako posodobite lastnosti predmeta aplikacije.
- [Zagotavljanje skrbniškega soglasja](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – za soglasje skrbnika in splošno soglasje potrebujemo, da skrbnik izrecno podeli soglasje.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – vsebnik upravljanja vlog za enotne definicije vlog in dodelitve vlog za ponudnike RBAC Microsoft 365 ki podpirajo več glavnic in več obsegov v eni dodelitvi vloge. Ta se razlikuje od *vrste vira rbacApplication.* Microsoft Intune je primer takšnega ponudnika RBAC. Dodelitev vloge v intune ima lahko matriko glavnega mesta in obseg skupin. **To je v beta različici, kar pomeni, da je še vedno v razvoju in ga ne priporočamo za uporabo v produkciji.**
