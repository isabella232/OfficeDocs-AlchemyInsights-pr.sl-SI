---
title: Sinhronizacija gesel za gesla za storitev Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177621"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sinhronizacija gesel za gesla za storitev Domain

**Če je vaš primerek Azure AD DS nastavljen tako, da omogočite sinhronizacijo z geslom**

Naletite na scenarij, v katerem izvajate hibridno okolje z uporabniki, ki se sinhronizirajo z okoljem domenskih storitev Azure Active Directory (AD DS) na mestu uporabe. Ta postopek je naletel, kljub temu, da imate na mestu AD DS na mestu uporabe možnost sinhronizacije gesla, s svojim najemnikom storitve Azure AD.

**Ker**

To se dogaja, ker Azure AD Connect by default ne sinhronizira podedovane nove tehnologije LAN upravitelja (NTLM) in Kerberos password, ki so potrebni za Azure AD DS.

**Rešitev** 

Če želite sinhronizirati gesla, potrebna za preverjanje pristnosti protokola NTLM in Kerberos, morate konfigurirati povezavo s storitvijo Azure AD.

Ko je konfiguracija storitve Azure AD Connect konfigurirana, se ustvari račun na mestu uporabe ali dogodek spremembe gesla, nato pa sinhronizira podedovano geslo v storitvi Azure AD. Če želite več informacij o tem in navodila za omogočanje sinhronizacije gesel v hibridnih okoljih storitve Azure AD DS, si oglejte [tukaj](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) .