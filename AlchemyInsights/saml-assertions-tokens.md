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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="30515-102">SAML trditve (žetoni)</span><span class="sxs-lookup"><span data-stu-id="30515-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="30515-103">Žetoni za označevanje varnostnih znakov (SAML) so XML, ki predstavljajo terjatve.</span><span class="sxs-lookup"><span data-stu-id="30515-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="30515-104">Privzeto so SAML žetoni za Windows Communication Foundation (WCF) v zveznih varnostnih scenarijih izdani žetoni.</span><span class="sxs-lookup"><span data-stu-id="30515-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="30515-105">Če želite več informacij, glejte [SAML žetoni in terjatve](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="30515-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="30515-106">Platforma Microsoft Identity oddaja več vrst varnostnih žetonov pri obdelavi posameznega toka preverjanja pristnosti.</span><span class="sxs-lookup"><span data-stu-id="30515-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="30515-107">[Sklici na SAML žetona](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) opisujejo obliko, varnostne značilnosti in vsebino žetonov SAML 2,0.</span><span class="sxs-lookup"><span data-stu-id="30515-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="30515-108">Upoštevajte navodila v napravah, ki jih je mogoče [konfigurirati v sistemu Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , da razumete, kako konfigurirate življenjske dobe žetona.</span><span class="sxs-lookup"><span data-stu-id="30515-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="30515-109">Upoštevajte navodila, opisana v [tem članku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , da razumete, kako konfigurirate šifriranje SAML žetona Azure ad.</span><span class="sxs-lookup"><span data-stu-id="30515-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="30515-110">V storitvi Azure AD lahko nastavite možnosti podpisovanja potrdil in algoritma za podpis potrdila.</span><span class="sxs-lookup"><span data-stu-id="30515-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="30515-111">Če želite več informacij, glejte [napredne možnosti podpisovanja potrdil v SAML žeton za aplikacije Gallery v imeniku Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="30515-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
