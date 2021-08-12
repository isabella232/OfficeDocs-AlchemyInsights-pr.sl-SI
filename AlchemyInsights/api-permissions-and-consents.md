---
title: Dovoljenja in soglasje ZA API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932113"
---
# <a name="api-permissions-and-consent"></a>Dovoljenja in soglasje ZA API

Aplikacije, ki so integrirane s Microsoftova platforma za identitete, vključujejo model avtorizacije, ki uporabnikom in skrbnikom omogoča nadzor nad tem, kako je mogoče dostopati do podatkov. Izvedba modela avtorizacije je bila posodobljena v končni Microsoftova platforma za identitete končni točki. Spremeni način interakcije aplikacije z Microsoftova platforma za identitete. [Dovoljenja in soglasje v končni Microsoftova platforma za identitete vključuje](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) osnovne koncepte tega modela avtorizacije, vključno z obsegi, dovoljenji in soglasjem.

Ogrodje [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) omogoča preprost razvoj spletnih in izvornih odjemalskih aplikacij z več najemniki. Te aplikacije omogočajo vpis z uporabniškimi računi iz najemnika Azure AD, ki je drugačen od tistega, v katerem je registrirana aplikacija. Poleg lastnih API-jev v spletu bodo morda potrebovali tudi spletne API-je, kot je API za Microsoft Graph (za dostop do storitev Azure AD, Intune in storitev v strežniku Microsoft 365) in drugih API-jev Microsoftove storitve.

