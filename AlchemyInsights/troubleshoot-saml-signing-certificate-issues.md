---
title: Odpravljanje težav z SAML podpisom potrdil
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694450"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Odpravljanje težav z SAML podpisom potrdil

Če želite odpraviti težavo s podpisom potrdila SAML, izvedite te priporočene korake:

1. Ko dodate program za podjetja, ki podpira SSO, bo Azure ustvaril potrdilo, ki se imenuje [SAML podpisno potrdilo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). To potrdilo ima rok trajanja 3 leta. Če želite spremeniti datum poteka potrdila, si oglejte [prilagajanje datuma poteka za potrdilo o poteku veljavnosti potrdila o poteku in ga prepeljite v novo potrdilo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure bo s tem potrdilom podpisal žetone SAML, ki jih zahteva aplikacija, in ga poslal v program za uspešno SSO. Če želite, da se to dokonča, prenesite potrdilo iz portala Azure in ga pošljite prodajalcu programov, da dokončate postopek SSO.

Ko je ta postopek končan, bo aplikacija zaupala temu potrdilu in vsi SAML žetoni, ki jih podpiše to potrdilo, bodo sprejeli program.

3. Če to potrdilo poteče, ustvarite novo potrdilo, ga posodobite na prodajalca aplikacij in ga nato naredite na strani Azure Side. Če želite več informacij, glejte [podaljšanje potrdila, ki bo kmalu potekla](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Če potrdilo poteče, uporabnik ne bo blokiran.

4. [Dodajanje e-poštnega naslova za obvestila](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , ki bodo prejeta, preden potek trenutnega potrdila poteče.

> [!NOTE]
> Step-4 je izbirna ena.

5. Spremenite možnosti podpisa potrdila programa SAML in algoritem za podpis potrdila. Če želite več informacij, glejte [Spreminjanje možnosti podpisovanja potrdil in algoritma za podpis](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

