---
title: Kako dodati in upravljati adminstrators – priporočene korake
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678871"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Kako dodati in upravljati adminstrators – priporočene korake

**Urejanje upravitelja naročnine ali soskrbnika**

- Skrbnik računa lahko ureja obe vlogi, medtem ko lahko skrbnik naročnine spremeni le soskrbnike v [portalu Azure](https://ms.portal.azure.com/#home).
- [Dodajanje ali spreminjanje skrbnikov naročnine na Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Posodobitev skrbnika naročnine ali Co-Administrator za notranje (AIRS) naročnine**

Skrbnik storitve ali soskrbnik lahko to dejanje samouporabi s temi koraki:

1. Prijavite se v [portal Azure](https://ms.portal.azure.com/#home) in kliknite **upravljanje stroškov + obračunavanje** v levem rezilu.
2. Kliknite element vrstice z naročnino. S tem odprete pregled naročnine.
3. Na rezilu **naročnine** kliknite **lastnosti**. 
4. Kliknite gumb» **skrbnik storitve** «.
5. Vnesite e-poštno sporočilo uporabnika, ki ga želite nastaviti kot skrbnika storitve, in kliknite **v redu**.

**Dodajanje/spreminjanje/odstranjevanje soskrbnika**

1. Prijavite se v [portal Azure](https://ms.portal.azure.com/#home) kot skrbnik storitve.
2. Odpiranje [naročnin](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in izbiranje naročnine. (Adminstrators lahko dodelite le na obseg naročnine.)
3. Pomaknite se do razdelka» **nadzor dostopa «(iam) –**  >  **klasični skrbniki**  >  **dodajte**  >  **Dodajanje soskrbnika** , da odprete podokno **Dodajanje** soodločanja (če je možnost Dodaj soskrbnika onemogočena, to pomeni, da nimate dovoljenj).
4. Izberite uporabnika, ki ga želite dodati, in kliknite **Dodaj**.

**več:**
- [Dodajanje soskrbnika](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Odstranjevanje soskrbnika](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Spreminjanje skrbnika storitve](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ogled skrbnika računa](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Upravljanje dostopa s portalom» RBAC «in» Azure «](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Dodajanje/brisanje uporabnikov z imenikom Azure Active Directory (AD)**

Dodate lahko nove uporabnike ali izbrišete obstoječe uporabnike iz organizacije Azure Active Directory (Azure AD):

1. Če želite dodati novega uporabnika, se prijavite v [portal Azure](https://ms.portal.azure.com/#home) kot uporabnik – skrbnik organizacije.
2. Izberite **Azure Active Directory**, izberite **Uporabniki** in nato kliknite **nov uporabnik**.
3. Na strani **uporabnik** izpolnite zahtevane informacije. Kliknite **Ustvari**. Uporabnik je ustvarjen in dodan v najemnika v storitvi Azure AD.

**Več informacij**:

- [Dodajanje novega uporabnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Brisanje uporabnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Dodajanje ali posodabljanje uporabnikovih podatkov profila v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Priporočeni dokumenti**

- [Kaj je nadzor dostopa na podlagi vloge (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Razumevanje različnih vlog v storitvi Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Dovoljenja skrbnika za vlogo v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Vadnica: dodeljevanje dostopa uporabniku z uporabo RBAC in portala Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Odpravljanje težav s RBAC v storitvi Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizirajte vire s skupinami za upravljanje Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kako zaprositi ulitek od Azure račun pot email](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Dodajanje, posodabljanje ali odstranjevanje kreditne ali debetne kartice v storitvi Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Upravljanje naročnine (vnovična aktivacija/preklic/preklop)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



