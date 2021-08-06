---
title: Dostop z naročnino
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
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999256"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Zaradi težav z brskalnikom se ni mogoče vpisati v Azure (brskalnik se obesi, vrteč se ne naloži itn.)

Morda bo to vplivalo na vas. Preverite, ali trenutno ni na voljo: stanje [storitve Azure Health.](https://status.azure.com/status/history/)

Odjavi se iz vseh aktivnih sej Azure. Zaženite zasebni način ali način brez beleženja zgodovine spletnega brskalnika.

Lahko tudi poskusite osvežiti brskalnik, uporabite drug brskalnik in izbrišete piškotke predpomnilnika, če zgoraj ne deluje.

Več informacij: [Odpravljanje težav z vpisom](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Dostop do naročnin ni uspel**

V [portalu Azure preverite,](https://portal.azure.com/)ali je v računu zgoraj desno izbran pravilen imenik Azure.

V [središču za račun Azure](https://account.windowsazure.com/Subscriptions)preverite, ali je račun, uporabljen za skrbnika računa.

Več informacij: Odpravljanje [težav z naročninami ni bilo mogoče najti](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Do zgodovine obračunavanja ni mogoče dostopati**

Skrbnik računa mora zagotovite, da je uporabnik, ki dostopa do podatkov za obračunavanje, dodan v imenik Azure Active directory kot gostujo uporabnik: Dodajte ali [izbrišite novega uporabnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Uporabnik mora imeti vlogo globalnega skrbnika: [Dodelite vlogo uporabnikom.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Objavite to možnost, uporabniku lahko dodelite dostop za obračunavanje s pravilniki za RBAC: [Podelitev dovoljenja za dostop do obračunavanja.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Priporočeni dokumenti**

-   [Ne morem se vpisati za upravljanje naročnine na Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)