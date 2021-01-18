---
title: Konfiguracija protokola LDAP
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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885578"
---
# <a name="configure-ldap"></a>Konfiguracija protokola LDAP

Če želite konfigurirati protokol LDAP, naredite to:

1. Preverite stanje domene na [portalu Azure](https://aka.ms/aadds-health).
1. Zagotovite, da je na voljo veljavna naročnina na Azure AD in je omogočena storitev Azure AD Domain Services.
1. Potrdilo, ki je zahtevano za omogočanje varnega LDAP, mora biti pridobljeno iz zaupanja vrednega javnega overovitelja ali pa je samopodpisano potrdilo.
1. Zagotovite, da bo potrdilo sledilo zahtevanim [navodilom](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Neveljavno potrdilo**
1. Če želite obnoviti potrdilo, upoštevajte navodila za ustvarjanje novega potrdila in reupload: [Konfiguriranje protokola LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Če želite razrešiti znano težavo z varnimi opozorili LDAP v domenskih storitvah storitve Azure Active Directory, glejte [Odpravljanje opozoril LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
