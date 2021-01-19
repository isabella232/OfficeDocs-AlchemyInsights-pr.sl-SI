---
title: Odpravljanje težav z gostujočimi Uporabniki
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901590"
---
# <a name="troubleshoot-guest-user-issues"></a>Odpravljanje težav z gostujočimi Uporabniki

1. Če želite navodila za upravljanje dostopa za goste do programov, glejte [upravljanje dostopa za goste s pregledi za dostop do storitve AZURE ad](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Dodajte gostujoče uporabnike v imenik v portalu Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): v tem hitrim vodniku boste v imenik Azure ad dodali novega gostujočega uporabnika prek portala Azure, poslali povabilo in si ogledali postopek odkupa povabila gostujočega uporabnika.
1. [Dodajanje gostujočega uporabnika z lupino PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): v tem hitrim vodniku boste uporabili ukaz New-AzureADMSInvitation, da dodate enega gostujočega uporabnika v svojega najemnika v storitvi Azure.
1. Če želite izvedeti več o dodeljevanju uporabnikov in skupin v aplikacije Enterprise v imeniku Azure Active Directory (Azure AD), ki je na portalu Azure ali z uporabo lupine PowerShell, glejte [upravljanje dodelitve uporabnika za program v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Sodelovanje z imenikom Azure Active Directory (Azure AD) B2B deluje z večino aplikacij, ki so integrirane v storitvi Azure AD. V tem [članku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)se sprehajamo po navodilih za konfiguriranje nekaterih priljubljenih aplikacij SaaS za uporabo s storitvijo AZURE ad B2B.
1. Kot organizacija, ki uporablja zmogljivosti za sodelovanje v storitvi Azure Active Directory (Azure AD) B2B, da povabi gostujoče uporabnike iz partnerskih organizacij v vaš oglas Azure, lahko zdaj uporabnikom teh B2B omogočite dostop do aplikacij na mestu uporabe. Ti programi na mestu uporabe lahko uporabljajo SAML preverjanje pristnosti ali integrirano preverjanje pristnosti sistema Windows (IWA) s omejena pooblastila Kerberos (KCD). Če želite več informacij, glejte [dodeljevanje uporabnikov storitve B2B v storitvi AZURE ad dostop do aplikacij na mestu uporabe](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Naučite se [dodeliti dostop do virov v oblaku z uporabo storitve AZURE ad B2B s sodelovanjem v lokalnem upravljanem partnerju](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).