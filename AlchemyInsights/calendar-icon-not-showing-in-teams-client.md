---
title: Ikona koledarja ni prikazana v odjemalcu aplikacije Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989607"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona koledarja ni prikazana v odjemalcu aplikacije Teams

Zavihek »Koledar« v aplikaciji Teams zahteva dostop do nabiralnika Exchange prek storitev Exchange Web Services. Nabiralnik Exchange je lahko v spletu ali na mestu uporabe. Za spletne uporabnike, ki ne vidijo zavihka »Koledar«, preverite, [ali imajo licenco za nabiralnik Exchange Online in ali je nabiralnik omogočen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Če ima uporabnik veljaven nabiralnik v storitvi Exchange Online, vendar še vedno ne vidi zavihka »Koledar«, je morda prišlo do težave z omrežjem. Uporabite [Microsoftov analizator oddaljene povezljivosti](https://testconnectivity.microsoft.com/) in zaženite **preskuse povezljivosti z Microsoft Exchangeevimi spletnimi storitvami** za prizadetega uporabnika.

Na koncu preverite še [Aplikacije Teams – pravilniki o nastavitvah aplikacij](https://admin.teams.microsoft.com/policies/app-setup) in se prepričajte, da aplikacija Koledar ni bila odstranjena iz pravilnika, uporabljenega za uporabnika (najverjetneje **Globalno (privzeto na ravni celotne organizacije)**.

Če vaši uporabniki uporabljajo aplikacije na mestu uporabe, morate preveriti, ali je hibridna konfiguracija ustrezna. Za odpravljanje težav uporabite [čarovnika za hibridno konfiguracijo](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Imejte v mislih, da [aplikacija Teams zahteva Exchange 2016 CU3 ali višje](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
