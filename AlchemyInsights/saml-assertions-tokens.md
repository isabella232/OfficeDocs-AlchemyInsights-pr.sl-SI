---
title: SAML trditve (žetoni)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885676"
---
# <a name="saml-assertions-tokens"></a>SAML trditve (žetoni)

1. Žetoni za označevanje varnostnih znakov (SAML) so XML, ki predstavljajo terjatve. Privzeto so SAML žetoni za Windows Communication Foundation (WCF) v zveznih varnostnih scenarijih izdani žetoni. Če želite več informacij, glejte [SAML žetoni in terjatve](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Platforma Microsoft Identity oddaja več vrst varnostnih žetonov pri obdelavi posameznega toka preverjanja pristnosti. [Sklici na SAML žetona](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) opisujejo obliko, varnostne značilnosti in vsebino žetonov SAML 2,0.
3. Upoštevajte navodila v napravah, ki jih je mogoče [konfigurirati v sistemu Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , da razumete, kako konfigurirate življenjske dobe žetona.
4. Upoštevajte navodila, opisana v [tem članku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , da razumete, kako konfigurirate šifriranje SAML žetona Azure ad.
5. V storitvi Azure AD lahko nastavite možnosti podpisovanja potrdil in algoritma za podpis potrdila. Če želite več informacij, glejte [napredne možnosti podpisovanja potrdil v SAML žeton za aplikacije Gallery v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
