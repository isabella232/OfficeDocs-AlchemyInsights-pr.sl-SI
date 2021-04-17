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
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819969"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona koledarja ni prikazana v odjemalcu aplikacije Teams

Zavihek »Koledar« v aplikaciji Teams zahteva dostop do nabiralnika Exchange prek storitev Exchange Web Services. Nabiralnik Exchange je lahko v spletu ali na mestu uporabe. Za spletne uporabnike, ki ne vidijo zavihka »Koledar«, preverite, [ali imajo licenco za nabiralnik Exchange Online in ali je nabiralnik omogočen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Če ima uporabnik veljaven nabiralnik v storitvi Exchange Online, vendar še vedno ne vidi zavihka »Koledar«, je morda prišlo do težave z omrežjem. Uporabite [Microsoftov analizator oddaljene povezljivosti](https://testconnectivity.microsoft.com/) in zaženite **preskuse povezljivosti z Microsoft Exchangeevimi spletnimi storitvami** za prizadetega uporabnika.

Na koncu preverite še [Aplikacije Teams – pravilniki o nastavitvah aplikacij](https://admin.teams.microsoft.com/policies/app-setup) in se prepričajte, da aplikacija Koledar ni bila odstranjena iz pravilnika, uporabljenega za uporabnika (najverjetneje **Globalno (privzeto na ravni celotne organizacije)**.

Če vaši uporabniki uporabljajo aplikacije na mestu uporabe, morate preveriti, ali je hibridna konfiguracija ustrezna. Za odpravljanje težav uporabite [čarovnika za hibridno konfiguracijo](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Imejte v mislih, da [aplikacija Teams zahteva Exchange 2016 CU3 ali višje](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
