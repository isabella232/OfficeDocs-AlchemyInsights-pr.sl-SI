---
title: Konfiguracija pravilnika LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090428"
---
# <a name="configure-ldap"></a>Konfiguracija pravilnika LDAP

Če želite konfigurirati pravilnik LDAP, naredite to:

1. Preverite stanje domene na [portalu Azure.](https://aka.ms/aadds-health)
1. Preverite, ali je na voljo veljavna naročnina na Azure AD in da so omogočene domenske storitve Azure AD.
1. Potrdilo, ki je zahtevano za omogočanje varnih potrdil LDAP, morate pridobiti pri zaupanja vrednem javnem overitelju digitalnih potrdil ali samopodpisano potrdilo.
1. Prepričajte se, da potrdilo upošteva zahtevane [smernice.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Neveljavno potrdilo**
1. Če želite podaljšati potrdilo, upoštevajte navodila za ustvarjanje novega potrdila in ponovno nalaganje: [konfigurirajte LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Če želite odpraviti znano težavo z opozorili varnega pravilnika LDAP v domenskih storitvah Azure Active Directory, glejte [Razreševanje opozoril pravilnika LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
