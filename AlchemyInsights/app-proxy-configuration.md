---
title: Konfiguracija proxyja aplikacije
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885528"
---
# <a name="app-proxy-configuration"></a>Konfiguracija proxyja aplikacije

1. Če želite razumeti, kako konfigurirate program proxy programa v storitvi Azure AD, da razkrijete aplikacije na mestu uporabe v oblaku, glejte [Kako konfigurirate program proxy programa](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Enotna prijava (SSO) uporabnikom omogoča dostop do aplikacije brez preverjanja pristnosti večkrat. Omogoča enotno preverjanje pristnosti, ki se pojavi v oblaku, proti imeniku Azure Active Directory, in dovoljuje storitvi ali povezovalniku, da pozove uporabnika, da dokonča vse dodatne izzive preverjanja pristnosti iz aplikacije. Če želite izvedeti več, si oglejte [kako konfigurirati enotno prijavo v program proxy programa](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. S [tem člankom](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) lahko odpravite težave s pogostimi težavami, ko ustvarjate nov program proxy strežnika.
4. Če imate težave z vzpostavljanjem preverjanja pristnosti, ki je na voljo v aplikaciji, boste morda morali [odpraviti omejitve dodeljevanja strežnikov Kerberos za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ali pa upoštevajte navodila za [konfiguracijo aplikacije s PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) , da odpravite težavo.
