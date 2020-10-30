---
title: Dostop do naročnine
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807722"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Ne morem se vpisati v Azure zaradi težav z brskalnikom (brskalnik se obesi, se vrti, ne naloži, itd.)

Morda boste vplivali na izpad. Preverite, ali je prišlo do trajnega izpada: [stanje Azure Health](https://status.azure.com/status/history/).

Odjavite se iz vseh aktivnih sej v storitvi Azure. Začnite v zasebnem ali načinu brez beleženja zgodovine v spletnem brskalniku.

Lahko tudi poskusite osvežiti brskalnik, uporabite drug brskalnik, izbrišete piškotke predpomnilnika, če zgoraj ne deluje.

Več informacij: [Odpravljanje težav z vpisom](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Dostop do naročnin ni mogoč**

V [portalu Azure](https://portal.azure.com/)se prepričajte, da je na računu v zgornjem desnem kotu izbran pravilen imenik Azure.

V [središču za Azure Account (račun](https://account.windowsazure.com/Subscriptions)) se prepričajte, ali je račun uporabljen pri skrbniku računa.

Več informacij: [Odpravljanje težav z naročnino](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dostop do zgodovine obračunavanja ni mogoč**

Skrbnik računa mora preveriti, ali je uporabnik, ki dostopa do informacij o obračunavanju, dodan v imeniku Azure Active Directory kot gostujoči uporabnik: [Dodajanje ali brisanje novega uporabnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Uporabnik mora nato dati globalno skrbniško vlogo: [dodeliti vlogo uporabnikom](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Objavite to, uporabniku je mogoče dodeliti dostop do obračunavanja s pravilniki RBAC: [dodeljevanje dostopa do obračunavanja](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Priporočeni dokumenti**

-   [Ne morem se vpisati v upravljanje moje naročnine na Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)