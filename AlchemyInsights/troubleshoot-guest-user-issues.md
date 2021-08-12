---
title: Odpravljanje težav z gostujo uporabniki
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939395"
---
# <a name="troubleshoot-guest-user-issues"></a>Odpravljanje težav z gostujo uporabniki

1. Če želite navodila o upravljanju dostopa za goste do aplikacij, glejte [Upravljanje dostopa za goste z mnenji](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)o dostopu za Azure AD.
1. [Dodajte gostujoče](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)uporabnike v imenik na portalu Azure: V tem vodniku za hitri začetek boste dodali novega gostujočega uporabnika v imenik Azure AD prek portala Azure, poslali povabilo in si videli, kako je videti postopek za unovčenje povabil gostužnega uporabnika.
1. [Dodajanje gostužnega uporabnika](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)z lupino PowerShell: V tem vodniku za hitri začetek boste uporabili New-AzureADMSInvitation za dodajanje enega gostužnega uporabnika v najemnika Azure.
1. Če želite izvedeti, kako dodelite uporabnike in skupine aplikacijam za podjetja v storitvi Azure Active Directory (Azure AD), bodisi v portalu Azure bodisi s storitvijo PowerShell, glejte Upravljanje dodelitve uporabnikov za aplikacijo v [storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory med podjetji v storitvi (Azure AD) deluje z večino aplikacij, ki so integrirane z imenikom Azure AD. V tem [članku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)so navodila za konfiguracijo nekaterih priljubljenih aplikacij SaaS za uporabo z imenikom Azure AD B2B.
1. Kot organizacija, ki uporablja zmogljivosti sodelovanja med podjetji v storitvi Azure Active Directory (Azure AD) za povabilo gostunje uporabnike iz partnerskih organizacij v imenik Azure AD, lahko tem uporabnikom B2B omogočite dostop do aplikacij na mestu uporabe. Ti programi na mestu uporabe lahko uporabljajo preverjanje pristnosti na osnovi SAML ali integrirano preverjanje pristnosti Windows (IWA) z omejenim pooblastilom Kerberos (KCD). Če želite več informacij, glejte Podelitev dovoljenja za dostop uporabnikov med [storitvijo B2B v](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)imeniku Azure AD do aplikacij na mestu uporabe.
1. Naučite se [dodeliti lokalno upravljanim partnerskim računom dostop do virov v](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)oblaku z uporabo sodelovanja med podjetji v storitvi Azure AD.