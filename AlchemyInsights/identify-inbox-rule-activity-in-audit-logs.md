---
title: Prepoznavanje dejavnosti pravila nabiralnika v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331139"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Prepoznavanje dejavnosti pravila nabiralnika v dnevnikih nadzora

Z iskanjem v dnevniku nadzora v Središče za skladnost okolja Microsoft 365 si ogledate dogodke pravila nabiralnika (ustvarjanje, spreminjanje in brisanje pravil nabiralnika).

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 <https://compliance.microsoft.com> pojdite na Nadzor  \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender pojdite <https://security.microsoft.com> na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://security.microsoft.com/auditlogsearch> .

2. Na **zavihku** Iskanje na **strani** Nadzor konfigurirajte te nastavitve:
   - **Datumski** in časovni obseg: Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - **Dejavnosti:** Izberite eno ali več teh vrednosti:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App.**
     - **Posodobitev pravil nabiralnika od Outlook odjemalca**

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja.

4. V rezultatih izberite dejavnost, da odprete letak s podrobnostmi. Informacije o nastavitvah pravila za mapo »Prejeto« so prikazane v **polju Parametri.**

Če želite več informacij, glejte [Določanje, ali je uporabnik ustvaril pravilo za mapo »Prejeto«.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
